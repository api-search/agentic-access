---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 13
api_specs:
- filename: alshhbaa-com-auth-api-openapi.yml
  format: yaml
  label: النحاسيات الشهباء Auth API
  slug: alshhbaa-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alshhbaa-com/openapi/alshhbaa-com-auth-api-openapi.yml
- filename: alshhbaa-com-consultations-api-openapi.yml
  format: yaml
  label: النحاسيات الشهباء Consultations API
  slug: alshhbaa-com-consultations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alshhbaa-com/openapi/alshhbaa-com-consultations-api-openapi.yml
- filename: alshhbaa-com-discovery-api-openapi.yml
  format: yaml
  label: النحاسيات الشهباء Discovery API
  slug: alshhbaa-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alshhbaa-com/openapi/alshhbaa-com-discovery-api-openapi.yml
- filename: alshhbaa-com-projects-api-openapi.yml
  format: yaml
  label: النحاسيات الشهباء Projects API
  slug: alshhbaa-com-projects-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/alshhbaa-com/openapi/alshhbaa-com-projects-api-openapi.yml
consequence_counts:
  read: 13
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Alshhbaa Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'النحاسيات الشهباء exposes 16 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: النحاسيات الشهباء
provider_slug: alshhbaa-com
slug: alshhbaa-com-agentic-access
source_filename: alshhbaa-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/alshhbaa-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 13\n    acting: 3\n  by_consequence:\n    read: 13\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /.well-known/api-catalog\n  method: get\n  operationId: getApiCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/agent-skills/index.json\n  method: get\n  operationId: getAgentSkillsIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /.well-known/mcp\n  method: get\n  operationId: getMcpDiscovery\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/mcp/server-card.json\n  method: get\n  operationId: getMcpServerCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/agent-card.json\n  method: get\n  operationId: getAgentCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-protected-resource\n  method: get\n  operationId: getOAuthProtectedResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-authorization-server\n  method: get\n \
  \ operationId: getOAuthAuthorizationServer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/ard.json\n  method: get\n  operationId: getAgenticResourceCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/ai-catalog.json\n  method: get\n  operationId: getAiCatalogAlias\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/http-message-signatures-directory\n  method: get\n  operationId: getBotAuthDirectory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ask\n  method: get\n  operationId: askDiscoveryGet\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ask\n  method: post\n  operationId: askDiscoveryPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp\n  method: post\n  operationId: callPublicMcpTool\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/summary\n  method: get\n  operationId: getApiV1Summary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/v1/projects\n  method: get\n  operationId: getApiV1Projects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/consultations\n  method: post\n  operationId: createApiV1Consultation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/alshhbaa-com/agentic-access/alshhbaa-com-agentic-access.yml
summary_line: 16 operations · 3 acting
tags:
- Lighting
- Chandeliers
- Saudi Arabia
- Luxury
- Manufacturing
- Company
---
