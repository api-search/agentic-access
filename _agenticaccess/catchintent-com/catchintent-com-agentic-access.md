---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 9
api_specs:
- filename: catchintent-com-discovery-api-openapi.yml
  format: yaml
  label: CatchIntent Discovery API
  slug: catchintent-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/catchintent-com/openapi/catchintent-com-discovery-api-openapi.yml
- filename: catchintent-com-health-api-openapi.yml
  format: yaml
  label: CatchIntent Health API
  slug: catchintent-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/catchintent-com/openapi/catchintent-com-health-api-openapi.yml
- filename: catchintent-com-mcp-api-openapi.yml
  format: yaml
  label: CatchIntent MCP API
  slug: catchintent-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/catchintent-com/openapi/catchintent-com-mcp-api-openapi.yml
- filename: catchintent-com-oauth-api-openapi.yml
  format: yaml
  label: CatchIntent OAuth API
  slug: catchintent-com-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/catchintent-com/openapi/catchintent-com-oauth-api-openapi.yml
consequence_counts:
  read: 9
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Catchintent Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'CatchIntent exposes 11 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CatchIntent
provider_slug: catchintent-com
slug: catchintent-com-agentic-access
source_filename: catchintent-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/catchintent-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    acting: 2\n    connected: 9\n  by_consequence:\n    write: 2\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /mcp\n  method: post\n  operationId: callMcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp\n  method: get\n  operationId: getMcpUnsupported\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n  method: delete\n  operationId: deleteMcpUnsupported\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /.well-known/oauth-protected-resource\n  method: get\n  operationId: getOAuthProtectedResourceMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-protected-resource/mcp\n  method: get\n  operationId: getOAuthProtectedResourceMetadataForMcp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-authorization-server\n  method:\
  \ get\n  operationId: getOAuthAuthorizationServerMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-authorization-server/mcp\n  method: get\n  operationId: getOAuthAuthorizationServerMetadataForMcp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/healthy\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/api-catalog\n  method: get\n  operationId: getApiCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/mcp/server-card.json\n  method: get\n  operationId: getMcpServerCard\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/agent-skills/index.json\n  method: get\n  operationId: getAgentSkillsIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/catchintent-com/agentic-access/catchintent-com-agentic-access.yml
summary_line: 11 operations · 2 acting
tags:
- B2B
- Sales
- Intent Data
- Artificial Intelligence
- Outbound
---
