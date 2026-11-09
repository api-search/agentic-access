---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 6
api_specs:
- filename: meatspace-run-keys-api-openapi.yml
  format: yaml
  label: meatspace-run Keys API
  slug: meatspace-run-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meatspace-run/openapi/meatspace-run-keys-api-openapi.yml
- filename: meatspace-run-mcp-api-openapi.yml
  format: yaml
  label: meatspace-run MCP API
  slug: meatspace-run-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meatspace-run/openapi/meatspace-run-mcp-api-openapi.yml
- filename: meatspace-run-requests-api-openapi.yml
  format: yaml
  label: meatspace-run Requests API
  slug: meatspace-run-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meatspace-run/openapi/meatspace-run-requests-api-openapi.yml
- filename: meatspace-run-review-api-openapi.yml
  format: yaml
  label: meatspace-run Review API
  slug: meatspace-run-review-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meatspace-run/openapi/meatspace-run-review-api-openapi.yml
- filename: meatspace-run-status-api-openapi.yml
  format: yaml
  label: meatspace-run Status API
  slug: meatspace-run-status-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/meatspace-run/openapi/meatspace-run-status-api-openapi.yml
consequence_counts:
  read: 6
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Meatspace Run Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'meatspace-run exposes 10 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: meatspace-run
provider_slug: meatspace-run
slug: meatspace-run-agentic-access
source_filename: meatspace-run-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/meatspace-run-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 4\n    connected: 6\n  by_consequence:\n    write: 4\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /api/keys\n  method: post\n  operationId: createApiKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/requests\n  method: post\n  operationId: createRequest\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/requests\n  method: get\n  operationId: listRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/requests/{id}\n  method: get\n  operationId: pollRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/requests/{id}\n  method: patch\n  operationId: submitResponse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /api/requests/{id}/wait\n  method: get\n  operationId: waitForResponse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/review/{id}\n  method: get\n  operationId: getReviewRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp\n  method: get\n  operationId: mcpServerInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp\n  method: post\n  operationId: mcpHandler\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /api/status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/meatspace-run/agentic-access/meatspace-run-agentic-access.yml
summary_line: 10 operations · 4 acting
tags:
- Company
- Artificial Intelligence
- Human-in-the-Loop
- Automation
---
