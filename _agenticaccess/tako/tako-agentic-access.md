---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 7
api_specs:
- filename: tako-openapi-original.yml
  format: yaml
  label: Tako Knowledge Search API
  slug: tako-knowledge-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tako/refs/heads/main/openapi/tako-openapi-original.yml
consequence_counts:
  read: 7
  write: 6
description: ''
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tako Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'Tako exposes 13 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Tako
provider_slug: tako
slug: tako-agentic-access
source_filename: tako-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/tako-openapi-original.yml\naudience: null\nnote: >-\n  Recommended x-agentic-access execution contracts, classified per operation from\n  the Tako OpenAPI (Curity Access Intelligence model). GET/HEAD → connected/read;\n  write-method POSTs → acting/write. No operation is payment/transfer/safety-critical\n  at the API-operation level (Tako's machine-payments surface is billing metadata,\n  not a transfer endpoint). A governance starting point, not an authoritative\n  provider claim.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 7\n    acting: 6\n  by_consequence:\n    read: 7\n    write: 6\n  human_in_the_loop: 0\n  audit_required: 6\noperations:\n  - operationId: graphSearch\n    method: GET\n    path: /beta/graph/search\n    action_class: connected\n    consequence: read\n    token: {ttl_seconds: 3600}\n  - operationId: graphRelated\n    method: GET\n    path: /beta/graph/related\n    action_class:\
  \ connected\n    consequence: read\n    token: {ttl_seconds: 3600}\n  - operationId: graphNode\n    method: GET\n    path: /beta/graph/node/{id}\n    action_class: connected\n    consequence: read\n    token: {ttl_seconds: 3600}\n  - operationId: listAnswerAgentRuns\n    method: GET\n    path: /v1/agent/answer/runs\n    action_class: connected\n    consequence: read\n    token: {ttl_seconds: 3600}\n  - operationId: getAnswerAgentRun\n    method: GET\n    path: /v1/agent/answer/runs/{run_id}\n    action_class: connected\n    consequence: read\n    token: {ttl_seconds: 3600}\n  - operationId: listRetrievalAgentRuns\n    method: GET\n    path: /v1/agent/retrieval/runs\n    action_class: connected\n    consequence: read\n    token: {ttl_seconds: 3600}\n  - operationId: getRetrievalAgentRun\n    method: GET\n    path: /v1/agent/retrieval/runs/{run_id}\n    action_class: connected\n    consequence: read\n    token: {ttl_seconds: 3600}\n  - operationId: search\n    method: POST\n    path: /v3/search\n\
  \    action_class: acting\n    consequence: write\n    token: {ttl_seconds: 900}\n    audit: required\n  - operationId: answer\n    method: POST\n    path: /v1/answer\n    action_class: acting\n    consequence: write\n    token: {ttl_seconds: 900}\n    audit: required\n  - operationId: contents\n    method: POST\n    path: /v1/contents\n    action_class: acting\n    consequence: write\n    token: {ttl_seconds: 900}\n    audit: required\n    note: Meters/bills a card CSV export beyond the free row allowance.\n  - operationId: createCard\n    method: POST\n    path: /v1/thin_viz/create/\n    action_class: acting\n    consequence: write\n    token: {ttl_seconds: 900}\n    audit: required\n  - operationId: createAnswerAgentRun\n    method: POST\n    path: /v1/agent/answer/runs\n    action_class: acting\n    consequence: write\n    token: {ttl_seconds: 900}\n    audit: required\n    note: PAYMENT_REQUIRED (402) pre-dispatch credit gate.\n  - operationId: createRetrievalAgentRun\n    method:\
  \ POST\n    path: /v1/agent/retrieval/runs\n    action_class: acting\n    consequence: write\n    token: {ttl_seconds: 900}\n    audit: required\n    note: PAYMENT_REQUIRED (402) pre-dispatch credit gate.\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tako/refs/heads/main/agentic-access/tako-agentic-access.yml
summary_line: 13 operations · 6 acting
tags:
- Company
- AI
- Data
- Search
- Answer Engine
- Financial Data
- Knowledge Graph
- Agents
- MCP
- Data Visualization
---
