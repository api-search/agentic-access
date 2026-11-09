---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 14
api_specs:
- filename: intentdocs-com-cli-api-openapi.yml
  format: yaml
  label: intentdocs-com CLI API
  slug: intentdocs-com-cli-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intentdocs-com/openapi/intentdocs-com-cli-api-openapi.yml
- filename: intentdocs-com-mcp-api-openapi.yml
  format: yaml
  label: intentdocs-com MCP API
  slug: intentdocs-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intentdocs-com/openapi/intentdocs-com-mcp-api-openapi.yml
- filename: intentdocs-com-oauth-api-openapi.yml
  format: yaml
  label: intentdocs-com OAuth API
  slug: intentdocs-com-oauth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intentdocs-com/openapi/intentdocs-com-oauth-api-openapi.yml
- filename: intentdocs-com-sync-api-openapi.yml
  format: yaml
  label: intentdocs-com Sync API
  slug: intentdocs-com-sync-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/intentdocs-com/openapi/intentdocs-com-sync-api-openapi.yml
consequence_counts:
  physical: 1
  read: 14
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Intentdocs Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/sync/{mapId}/build-order
operation_count: 28
overview: 'intentdocs-com exposes 28 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read, 13 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: intentdocs-com
provider_slug: intentdocs-com
slug: intentdocs-com-agentic-access
source_filename: intentdocs-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/intentdocs-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 28\n  by_action_class:\n    acting: 14\n    connected: 14\n  by_consequence:\n    write: 13\n    read: 14\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/cli/auth\n  method: post\n  operationId: createCliAuthRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/cli/auth\n  method: get\n  operationId: pollCliAuthStatus\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/cli/auth\n  method: put\n  operationId: approveCliAuthRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/cli/projects\n  method: get\n  operationId: listCliProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:projects\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/cli/projects/{projectId}/maps\n  method: get\n  operationId: listCliProjectMaps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:maps\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/oauth/authorize\n  method: get\n  operationId: oauthAuthorizeGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/oauth/authorize\n  method: post\n  operationId: oauthAuthorizePost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/oauth/token\n  method: post\n  operationId: oauthToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/oauth/token\n  method: options\n  operationId: oauthTokenOptions\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/oauth/register\n  method: post\n  operationId: oauthRegister\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/oauth/register\n  method: options\n  operationId: oauthRegisterOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-server\n  method: get\n  operationId: oauthServerMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-protected-resource\n\
  \  method: get\n  operationId: oauthResourceMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp\n  method: post\n  operationId: mcpPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - read:maps\n    - write:maps\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp\n  method: get\n  operationId: mcpGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:maps\n    - write:maps\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp\n  method: delete\n  operationId: mcpDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/sync/{mapId}/stories\n  method: get\n  operationId: listStories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/sync/{mapId}/stories\n  method: post\n  operationId: createStories\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/sync/{mapId}/stories\n  method: patch\n  operationId: updateStories\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/sync/{mapId}/context\n  method: get\n  operationId: getStoryMapContext\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/sync/{mapId}/activity\n  method: get\n  operationId: getRecentActivity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/sync/{mapId}/activity\n  method: post\n  operationId: logActivity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/sync/{mapId}/build-order\n  method: get\n  operationId:\
  \ getBuildOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/sync/{mapId}/build-order\n  method: put\n  operationId: updateBuildOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/sync/{mapId}/blocker\n  method: post\n  operationId: raiseBlocker\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/sync/{mapId}/decisions\n  method: get\n  operationId:\
  \ listDecisions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/sync/{mapId}/decisions\n  method: post\n  operationId: logDecision\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/sync/{mapId}/screenshots\n  method: post\n  operationId: uploadScreenshot\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/intentdocs-com/agentic-access/intentdocs-com-agentic-access.yml
summary_line: 28 operations · 14 acting
tags:
- Company
- Artificial Intelligence
- Spec-Driven
- Platform
- Automation
- Low-Code
---
