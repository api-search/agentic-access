---
acting_count: 0
action_class_counts:
  connected: 10
api_specs:
- filename: automq-ai-info-api-openapi.yml
  format: yaml
  label: AutoMQ Ai Info API
  slug: automq-ai-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automq/refs/heads/main/openapi/automq-ai-info-api-openapi.yml
- filename: automq-llms-full-txt-api-openapi.yml
  format: yaml
  label: AutoMQ Llms Full.txt API
  slug: automq-llms-full-txt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automq/refs/heads/main/openapi/automq-llms-full-txt-api-openapi.yml
- filename: automq-llms-txt-api-openapi.yml
  format: yaml
  label: AutoMQ Llms.txt API
  slug: automq-llms-txt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automq/refs/heads/main/openapi/automq-llms-txt-api-openapi.yml
- filename: automq-robots-txt-api-openapi.yml
  format: yaml
  label: AutoMQ Robots.txt API
  slug: automq-robots-txt-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automq/refs/heads/main/openapi/automq-robots-txt-api-openapi.yml
- filename: automq-well-known-api-openapi.yml
  format: yaml
  label: AutoMQ .well Known API
  slug: automq-well-known-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/automq/refs/heads/main/openapi/automq-well-known-api-openapi.yml
consequence_counts:
  read: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Automq Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'AutoMQ exposes 10 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AutoMQ
provider_slug: automq
slug: automq-agentic-access
source_filename: automq-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: generated\nsource: openapi/automq-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 10\n  by_consequence:\n    read: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /.well-known/api-catalog\n  method: get\n  operationId: getApiCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/openapi.json\n  method: get\n  operationId: getPublicDiscoveryOpenApi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/api-status\n  method:\
  \ get\n  operationId: getPublicDiscoveryStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/oauth-protected-resource\n  method: get\n  operationId: getOAuthProtectedResourceMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/mcp/server-card.json\n  method: get\n  operationId: getMcpServerCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/agent-skills/index.json\n  method: get\n  operationId: getAgentSkillsIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /robots.txt\n  method: get\n  operationId: getRobotsTxt\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms.txt\n  method: get\n  operationId: getLlmsIndex\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms-full.txt\n  method: get\n  operationId: getLlmsFullContext\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ai-info\n  method: get\n  operationId: getAiInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/automq/refs/heads/main/agentic-access/automq-agentic-access.yml
summary_line: 10 operations
tags:
- Company
- Kafka
- Streaming
- Event Streaming
- Object Storage
- Open Source
- Cloud
---
