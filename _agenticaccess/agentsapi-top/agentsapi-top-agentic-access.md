---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 15
api_specs:
- filename: agentsapi-top-alerts-api-openapi.yml
  format: yaml
  label: agentsapi-top Alerts API
  slug: agentsapi-top-alerts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsapi-top/openapi/agentsapi-top-alerts-api-openapi.yml
- filename: agentsapi-top-cctp-api-openapi.yml
  format: yaml
  label: agentsapi-top Cctp API
  slug: agentsapi-top-cctp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsapi-top/openapi/agentsapi-top-cctp-api-openapi.yml
- filename: agentsapi-top-cluster-api-openapi.yml
  format: yaml
  label: agentsapi-top Cluster API
  slug: agentsapi-top-cluster-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsapi-top/openapi/agentsapi-top-cluster-api-openapi.yml
- filename: agentsapi-top-explain-api-openapi.yml
  format: yaml
  label: agentsapi-top Explain API
  slug: agentsapi-top-explain-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsapi-top/openapi/agentsapi-top-explain-api-openapi.yml
- filename: agentsapi-top-filings-api-openapi.yml
  format: yaml
  label: agentsapi-top Filings API
  slug: agentsapi-top-filings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsapi-top/openapi/agentsapi-top-filings-api-openapi.yml
- filename: agentsapi-top-healthz-api-openapi.yml
  format: yaml
  label: agentsapi-top Healthz API
  slug: agentsapi-top-healthz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsapi-top/openapi/agentsapi-top-healthz-api-openapi.yml
- filename: agentsapi-top-label-api-openapi.yml
  format: yaml
  label: agentsapi-top Label API
  slug: agentsapi-top-label-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsapi-top/openapi/agentsapi-top-label-api-openapi.yml
- filename: agentsapi-top-mcp-api-openapi.yml
  format: yaml
  label: agentsapi-top MCP API
  slug: agentsapi-top-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsapi-top/openapi/agentsapi-top-mcp-api-openapi.yml
- filename: agentsapi-top-me-api-openapi.yml
  format: yaml
  label: agentsapi-top Me API
  slug: agentsapi-top-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsapi-top/openapi/agentsapi-top-me-api-openapi.yml
- filename: agentsapi-top-statusz-api-openapi.yml
  format: yaml
  label: agentsapi-top Statusz API
  slug: agentsapi-top-statusz-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsapi-top/openapi/agentsapi-top-statusz-api-openapi.yml
- filename: agentsapi-top-subscription-api-openapi.yml
  format: yaml
  label: agentsapi-top Subscription API
  slug: agentsapi-top-subscription-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/agentsapi-top/openapi/agentsapi-top-subscription-api-openapi.yml
consequence_counts:
  read: 15
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Agentsapi Top Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 23
overview: 'agentsapi-top exposes 23 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: agentsapi-top
provider_slug: agentsapi-top
slug: agentsapi-top-agentic-access
source_filename: agentsapi-top-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/agentsapi-top-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 15\n    acting: 8\n  by_consequence:\n    read: 15\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/label/{address}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/label/{address}\n  method: post\n  operationId: op_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n    \
  \  triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/explain/{txHash}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/explain/{txHash}\n  method: post\n  operationId: op_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/cluster/{funder}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cluster/{funder}\n  method: post\n  operationId: op_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/track/cctp/{txHash}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/track/cctp/{txHash}\n  method: post\n  operationId: op_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/alerts\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/alerts\n  method: post\n  operationId: op_post\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/alerts/stats\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/alerts/stats\n  method: post\n  operationId: op_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/alerts/subscribe\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/filings/8k\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/filings/today\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /healthz\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /statusz\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/me\n  method: post\n  operationId: getMe_post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/label\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n  method: post\n  operationId: mcpRpc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp\n  method: get\n  operationId: mcpCardOrStream\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /.well-known/mcp.json\n  method: get\n  operationId: wellKnownMcpJson\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/agentsapi-top/agentic-access/agentsapi-top-agentic-access.yml
summary_line: 23 operations · 8 acting
tags:
- Blockchain
- Risk Intelligence
- Cryptocurrency
- On-Chain Data
---
