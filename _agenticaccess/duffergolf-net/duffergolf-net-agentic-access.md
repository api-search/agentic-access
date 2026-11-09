---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 14
api_specs:
- filename: duffergolf-net-a2a-api-openapi.yml
  format: yaml
  label: Duffer Golf A2a API
  slug: duffergolf-net-a2a-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/duffergolf-net/openapi/duffergolf-net-a2a-api-openapi.yml
- filename: duffergolf-net-auth-md-api-openapi.yml
  format: yaml
  label: Duffer Golf Auth.md API
  slug: duffergolf-net-auth-md-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/duffergolf-net/openapi/duffergolf-net-auth-md-api-openapi.yml
- filename: duffergolf-net-manifest-webmanifest-api-openapi.yml
  format: yaml
  label: Duffer Golf Manifest.webmanifest API
  slug: duffergolf-net-manifest-webmanifest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/duffergolf-net/openapi/duffergolf-net-manifest-webmanifest-api-openapi.yml
- filename: duffergolf-net-mcp-api-openapi.yml
  format: yaml
  label: Duffer Golf MCP API
  slug: duffergolf-net-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/duffergolf-net/openapi/duffergolf-net-mcp-api-openapi.yml
- filename: duffergolf-net-well-known-api-openapi.yml
  format: yaml
  label: Duffer Golf .well Known API
  slug: duffergolf-net-well-known-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/duffergolf-net/openapi/duffergolf-net-well-known-api-openapi.yml
consequence_counts:
  read: 14
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Duffergolf Net Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 18
overview: 'Duffer Golf exposes 18 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Duffer Golf
provider_slug: duffergolf-net
slug: duffergolf-net-agentic-access
source_filename: duffergolf-net-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: generated\nsource: openapi/duffergolf-net-openapi.json, openapi/duffergolf-net.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    acting: 4\n    connected: 14\n  by_consequence:\n    write: 4\n    read: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /mcp\n  method: post\n  operationId: post_mcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /a2a\n  method: post\n  operationId: post_a2a\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp\n  method: post\n  operationId: post_mcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /a2a\n  method: post\n  operationId: post_a2a\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /.well-known/mcp.json\n  method: get\n  operationId: get_well_known_mcp_json\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/mcp/server-card.json\n  method: get\n  operationId: get_well_known_mcp_server_card_json\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp/server-card\n  method: get\n  operationId: get_mcp_server_card\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/api-catalog\n  method: get\n  operationId: get_well_known_api_catalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/agent-skills/index.json\n  method: get\n  operationId: get_well_known_agent_skills_index_json\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/ai-catalog.json\n  method: get\n  operationId: get_well_known_ai_catalog_json\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-protected-resource\n  method: get\n  operationId: get_well_known_oauth_protected_resource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/agent-card.json\n  method: get\n  operationId: get_well_known_agent_card_json\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth.md\n  method: get\n  operationId: get_auth_md\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/openapi.json\n  method: get\n  operationId: get_well_known_openapi_json\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/security.txt\n  method: get\n  operationId: get_well_known_security_txt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /manifest.webmanifest\n  method: get\n  operationId: get_manifest_webmanifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/mcp-registry-auth\n  method: get\n  operationId: get_well_known_mcp_registry_auth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /.well-known/agent-skills/{skill}/SKILL.md\n  method: get\n  operationId: get_agent_skill\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/duffergolf-net/agentic-access/duffergolf-net-agentic-access.yml
summary_line: 18 operations · 4 acting
tags:
- Company
- Golf
- Simulator
- Hardware
- E-Commerce
---
