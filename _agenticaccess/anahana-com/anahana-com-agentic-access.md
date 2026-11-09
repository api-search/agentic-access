---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 17
api_specs:
- filename: anahana-com-discovery-api-openapi.yml
  format: yaml
  label: Anahana Discovery API
  slug: anahana-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anahana-com/openapi/anahana-com-discovery-api-openapi.yml
- filename: anahana-com-mcp-api-openapi.yml
  format: yaml
  label: Anahana MCP API
  slug: anahana-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anahana-com/openapi/anahana-com-mcp-api-openapi.yml
- filename: anahana-com-oauth-api-openapi.yml
  format: yaml
  label: Anahana OAuth API
  slug: anahana-com-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/anahana-com/openapi/anahana-com-oauth-api-openapi.yml
consequence_counts:
  read: 17
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Anahana Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 20
overview: 'Anahana exposes 20 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Anahana
provider_slug: anahana-com
slug: anahana-com-agentic-access
source_filename: anahana-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/anahana-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    acting: 3\n    connected: 17\n  by_consequence:\n    write: 3\n    read: 17\n  human_in_the_loop_required: 0\noperations:\n- path: /mcp\n  method: post\n  operationId: mcpJsonRpc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - read:content\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp\n  method: options\n  operationId: mcpPreflight\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp/register\n  method: post\n  operationId: registerClient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/authorize\n  method: get\n  operationId: authorize\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp/token\n  method: post\n  operationId: token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /.well-known/oauth-authorization-server\n  method: get\n  operationId: authorizationServerMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-protected-resource\n  method: get\n  operationId: protectedResourceMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/mcp/server-card.json\n  method: get\n  operationId: mcpServerCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/agents.md\n  method: get\n  operationId: agentsMd\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth.md\n  method: get\n  operationId:\
  \ authMd\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/agent-skills/index.json\n  method: get\n  operationId: agentSkillsIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/agent-skills/ai-agent-wellbeing.tar.gz\n  method: get\n  operationId: agentSkillWellbeingArchive\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/api-catalog\n  method: get\n  operationId: apiCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi.json\n  method: get\n  operationId: openapiDocument\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms.txt\n  method: get\n  operationId: llmsTxt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms-full.txt\n  method: get\n  operationId: llmsFullTxt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /content-index/manifest.json\n  method: get\n  operationId: contentIndexManifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /content-index/{lang}.json\n  method: get\n  operationId: contentIndexLanguage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /content-index/angel-numbers.json\n\
  \  method: get\n  operationId: contentIndexAngelNumbers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{path}\n  method: get\n  operationId: getPageAsMarkdown\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/anahana-com/agentic-access/anahana-com-agentic-access.yml
summary_line: 20 operations · 3 acting
tags:
- SpiritualWellness
- Personal Growth
- Astrology
- Meditation
- Yoga
---
