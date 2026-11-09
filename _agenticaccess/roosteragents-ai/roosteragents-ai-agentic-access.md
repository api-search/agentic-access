---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 5
api_specs:
- filename: roosteragents-ai-agent-readiness-api-openapi.yml
  format: yaml
  label: roosteragents-ai Agent Readiness API
  slug: roosteragents-ai-agent-readiness-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roosteragents-ai/openapi/roosteragents-ai-agent-readiness-api-openapi.yml
- filename: roosteragents-ai-gateway-api-openapi.yml
  format: yaml
  label: roosteragents-ai Gateway API
  slug: roosteragents-ai-gateway-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roosteragents-ai/openapi/roosteragents-ai-gateway-api-openapi.yml
- filename: roosteragents-ai-mcp-api-openapi.yml
  format: yaml
  label: roosteragents-ai MCP API
  slug: roosteragents-ai-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roosteragents-ai/openapi/roosteragents-ai-mcp-api-openapi.yml
- filename: roosteragents-ai-scan-api-openapi.yml
  format: yaml
  label: roosteragents-ai Scan API
  slug: roosteragents-ai-scan-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/roosteragents-ai/openapi/roosteragents-ai-scan-api-openapi.yml
consequence_counts:
  read: 5
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Roosteragents Ai Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'roosteragents-ai exposes 6 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: roosteragents-ai
provider_slug: roosteragents-ai
slug: roosteragents-ai-agentic-access
source_filename: roosteragents-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/roosteragents-ai-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 1\n    connected: 5\n  by_consequence:\n    write: 1\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /mcp\n  method: post\n  operationId: mcpCall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gateway/directory.json\n  method: get\n  operationId: listBusinesses\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gateway/businesses/{id}.json\n  method: get\n  operationId: getBusiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/agent-readiness\n  method: get\n  operationId: agent_readiness\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/scan\n  method: get\n  operationId: ai_visibility_scan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/scan/full\n  method: get\n  operationId: ai_visibility_scan_full\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/roosteragents-ai/agentic-access/roosteragents-ai-agentic-access.yml
summary_line: 6 operations · 1 acting
tags:
- Artificial Intelligence
- Marketing
- Automation
- Software-as-a-Service
- Data
---
