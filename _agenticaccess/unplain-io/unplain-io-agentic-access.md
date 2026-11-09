---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 10
api_specs:
- filename: unplain-io-discovery-api-openapi.yml
  format: yaml
  label: unplain-io Discovery API
  slug: unplain-io-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unplain-io/openapi/unplain-io-discovery-api-openapi.yml
- filename: unplain-io-feature-requests-api-openapi.yml
  format: yaml
  label: unplain-io Feature requests API
  slug: unplain-io-feature-requests-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unplain-io/openapi/unplain-io-feature-requests-api-openapi.yml
- filename: unplain-io-mcp-api-openapi.yml
  format: yaml
  label: unplain-io MCP API
  slug: unplain-io-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/unplain-io/openapi/unplain-io-mcp-api-openapi.yml
consequence_counts:
  physical: 2
  read: 10
  safety-critical: 2
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Unplain Io Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/mcp
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /api/mcp
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/mcp
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/mcp
operation_count: 20
overview: 'unplain-io exposes 20 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 6 write, 2 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: unplain-io
provider_slug: unplain-io
slug: unplain-io-agentic-access
source_filename: unplain-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/app-unplain-io-openapi.json, openapi/unplain-io-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    acting: 10\n    connected: 10\n  by_consequence:\n    physical: 2\n    read: 10\n    safety-critical: 2\n    write: 6\n  human_in_the_loop_required: 2\noperations:\n- path: /api/mcp\n  method: post\n  operationId: mcpRpc\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/mcp\n  method: get\n  operationId: mcpStream\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp\n  method: delete\n  operationId: mcpEndSession\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/features\n  method: get\n  operationId: listFeatureRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/features\n  method: post\n  operationId: submitFeatureRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/features/similar\n  method: get\n  operationId: findSimilarFeatureRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/features/{id}/vote\n  method: post\n  operationId: castFeatureVote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/features/{id}/vote\n  method: delete\n  operationId: removeFeatureVote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /openapi.json\n  method: get\n  operationId: getOpenApiDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/mcp.json\n  method: get\n  operationId: getMcpManifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp\n  method: post\n  operationId: mcpRpc\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/mcp\n  method: get\n  operationId: mcpStream\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/mcp\n  method: delete\n  operationId: mcpEndSession\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/features\n  method: get\n  operationId: listFeatureRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/features\n  method: post\n  operationId: submitFeatureRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/features/similar\n  method: get\n  operationId: findSimilarFeatureRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/features/{id}/vote\n  method: post\n  operationId: castFeatureVote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/features/{id}/vote\n  method: delete\n  operationId: removeFeatureVote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /openapi.json\n  method: get\n  operationId: getOpenApiDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/mcp.json\n  method: get\n  operationId: getMcpManifest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/unplain-io/agentic-access/unplain-io-agentic-access.yml
summary_line: 20 operations · 10 acting · 2 human-in-the-loop
tags:
- Company
- PDF
- Artificial Intelligence
- Marketing
- Software-as-a-Service
---
