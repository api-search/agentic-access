---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 12
api_specs:
- filename: joinsandwich-com-auth-api-openapi.yml
  format: yaml
  label: joinsandwich-com Auth API
  slug: joinsandwich-com-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinsandwich-com/openapi/joinsandwich-com-auth-api-openapi.yml
- filename: joinsandwich-com-community-api-openapi.yml
  format: yaml
  label: joinsandwich-com Community API
  slug: joinsandwich-com-community-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinsandwich-com/openapi/joinsandwich-com-community-api-openapi.yml
- filename: joinsandwich-com-content-api-openapi.yml
  format: yaml
  label: joinsandwich-com Content API
  slug: joinsandwich-com-content-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinsandwich-com/openapi/joinsandwich-com-content-api-openapi.yml
- filename: joinsandwich-com-discovery-api-openapi.yml
  format: yaml
  label: joinsandwich-com Discovery API
  slug: joinsandwich-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinsandwich-com/openapi/joinsandwich-com-discovery-api-openapi.yml
- filename: joinsandwich-com-mcp-api-openapi.yml
  format: yaml
  label: joinsandwich-com MCP API
  slug: joinsandwich-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinsandwich-com/openapi/joinsandwich-com-mcp-api-openapi.yml
- filename: joinsandwich-com-newsletter-api-openapi.yml
  format: yaml
  label: joinsandwich-com Newsletter API
  slug: joinsandwich-com-newsletter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/joinsandwich-com/openapi/joinsandwich-com-newsletter-api-openapi.yml
consequence_counts:
  read: 12
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Joinsandwich Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 17
overview: 'joinsandwich-com exposes 17 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: joinsandwich-com
provider_slug: joinsandwich-com
slug: joinsandwich-com-agentic-access
source_filename: joinsandwich-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/joinsandwich-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 17\n  by_action_class:\n    connected: 12\n    acting: 5\n  by_consequence:\n    read: 12\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /openapi.json\n  method: get\n  operationId: getOpenApi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agents.json\n  method: get\n  operationId: getAgentsManifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms.txt\n  method: get\n\
  \  operationId: getLlmsTxt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms-full.txt\n  method: get\n  operationId: getLlmsFullTxt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/api-catalog\n  method: get\n  operationId: getApiCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/mcp/server.json\n  method: get\n  operationId: getMcpServerJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/mcp.json\n  method: get\n  operationId: getMcpJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-authorization-server\n  method: get\n  operationId: getOauthAuthorizationServer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp\n  method: get\n  operationId: getPublicMcpMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp\n  method: post\n  operationId: postPublicMcp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/md\n  method: get\n  operationId: getMarkdownByAccept\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/newsletter\n  method: post\n  operationId: subscribeNewsletter\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/auth/me\n  method: get\n  operationId: getAuthMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/auth/session\n  method: post\n  operationId: createAuthSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /api/auth/signout\n  method: post\n  operationId: signOutSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/community\n  method: get\n  operationId: getCommunity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/community\n  method: post\n  operationId: postCommunity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/joinsandwich-com/agentic-access/joinsandwich-com-agentic-access.yml
summary_line: 17 operations · 5 acting
tags:
- Company
- Directory
- Caregiving
- Technology
---
