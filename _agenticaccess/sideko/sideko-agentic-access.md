---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 11
api_specs:
- filename: sideko-api-projects-api-openapi.yml
  format: yaml
  label: Sideko API Projects API
  slug: sideko-api-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sideko/refs/heads/main/openapi/sideko-api-projects-api-openapi.yml
- filename: sideko-api-versions-api-openapi.yml
  format: yaml
  label: Sideko API Versions API
  slug: sideko-api-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sideko/refs/heads/main/openapi/sideko-api-versions-api-openapi.yml
- filename: sideko-authentication-api-openapi.yml
  format: yaml
  label: Sideko Authentication API
  slug: sideko-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sideko/refs/heads/main/openapi/sideko-authentication-api-openapi.yml
- filename: sideko-documentation-api-openapi.yml
  format: yaml
  label: Sideko Documentation API
  slug: sideko-documentation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sideko/refs/heads/main/openapi/sideko-documentation-api-openapi.yml
- filename: sideko-linting-api-openapi.yml
  format: yaml
  label: Sideko Linting API
  slug: sideko-linting-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sideko/refs/heads/main/openapi/sideko-linting-api-openapi.yml
- filename: sideko-mcp-generation-api-openapi.yml
  format: yaml
  label: Sideko MCP Generation API
  slug: sideko-mcp-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sideko/refs/heads/main/openapi/sideko-mcp-generation-api-openapi.yml
- filename: sideko-mock-servers-api-openapi.yml
  format: yaml
  label: Sideko Mock Servers API
  slug: sideko-mock-servers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sideko/refs/heads/main/openapi/sideko-mock-servers-api-openapi.yml
- filename: sideko-sdk-generation-api-openapi.yml
  format: yaml
  label: Sideko SDK Generation API
  slug: sideko-sdk-generation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sideko/refs/heads/main/openapi/sideko-sdk-generation-api-openapi.yml
consequence_counts:
  physical: 2
  read: 11
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sideko Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api-projects/{projectId}/docs
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api-projects/{projectId}/mock-servers
operation_count: 23
overview: 'Sideko exposes 23 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 10 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Sideko
provider_slug: sideko
slug: sideko-agentic-access
source_filename: sideko-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/sideko-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 11\n    acting: 12\n  by_consequence:\n    read: 11\n    write: 10\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api-projects\n  method: get\n  operationId: listApiProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api-projects\n  method: post\n  operationId: createApiProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n  \
  \    human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api-projects/{projectId}\n  method: get\n  operationId: getApiProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api-projects/{projectId}\n  method: put\n  operationId: updateApiProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api-projects/{projectId}\n  method: delete\n  operationId: deleteApiProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api-projects/{projectId}/versions\n  method: get\n  operationId: listApiVersions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api-projects/{projectId}/versions\n  method: post\n  operationId: createApiVersion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api-projects/{projectId}/versions/{versionId}/download\n  method: get\n  operationId: downloadApiVersionSpec\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api-projects/{projectId}/lint\n  method: post\n  operationId:\
  \ lintApiProject\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api-projects/{projectId}/sdks\n  method: get\n  operationId: listSdkGenerations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api-projects/{projectId}/sdks\n  method: post\n  operationId: triggerSdkGeneration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api-projects/{projectId}/sdks/{sdkId}\n  method: get\n  operationId: getSdkGeneration\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api-projects/{projectId}/mcps\n  method: get\n  operationId: listMcpGenerations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api-projects/{projectId}/mcps\n  method: post\n  operationId: triggerMcpGeneration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api-projects/{projectId}/mcps/{mcpId}\n  method: get\n  operationId: getMcpGeneration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api-projects/{projectId}/docs\n\
  \  method: get\n  operationId: listDocumentationSites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api-projects/{projectId}/docs\n  method: post\n  operationId: deployDocumentationSite\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api-projects/{projectId}/mock-servers\n  method: get\n  operationId: listMockServers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api-projects/{projectId}/mock-servers\n  method: post\n  operationId: deployMockServer\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api-projects/{projectId}/mock-servers/{serverId}\n  method: delete\n  operationId: deleteMockServer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/api-keys\n  method: get\n  operationId: listApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/api-keys\n  method: post\n  operationId: createApiKey\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/api-keys/{keyId}\n  method: delete\n  operationId: deleteApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sideko/refs/heads/main/agentic-access/sideko-agentic-access.yml
summary_line: 23 operations · 12 acting
tags:
- CLI
- Documentation
- Mock Servers
- Platform
- SDK
- API Tooling
- SDK Generation
- MCP Generation
- Artificial Intelligence
- Hybrid Codegen
- OpenAPI Linting
---
