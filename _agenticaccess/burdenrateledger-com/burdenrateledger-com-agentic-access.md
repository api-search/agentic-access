---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 2
api_specs:
- filename: burdenrateledger-com-dataset-api-openapi.yml
  format: yaml
  label: burdenrateledger-com Dataset API
  slug: burdenrateledger-com-dataset-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/burdenrateledger-com/openapi/burdenrateledger-com-dataset-api-openapi.yml
- filename: burdenrateledger-com-mcp-api-openapi.yml
  format: yaml
  label: burdenrateledger-com MCP API
  slug: burdenrateledger-com-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/burdenrateledger-com/openapi/burdenrateledger-com-mcp-api-openapi.yml
consequence_counts:
  read: 2
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Burdenrateledger Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'burdenrateledger-com exposes 9 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: burdenrateledger-com
provider_slug: burdenrateledger-com
slug: burdenrateledger-com-agentic-access
source_filename: burdenrateledger-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/burdenrateledger-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    acting: 7\n    connected: 2\n  by_consequence:\n    write: 7\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /mcp/tools/dataset_columns\n  method: post\n  operationId: dataset_columns\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/dataset_search\n  method: post\n  operationId: dataset_search\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp/tools/dataset_row\n  method: post\n  operationId: dataset_row\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/dataset_compare\n  method: post\n  operationId: dataset_compare\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/dataset_stats\n  method: post\n  operationId: dataset_stats\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/dataset_top\n  method: post\n  operationId: dataset_top\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp/tools/dataset_provenance\n  method: post\n  operationId: dataset_provenance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp\n  method: post\n  operationId: mcp\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mcp\n  method: get\n  operationId: mcpCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/burdenrateledger-com/agentic-access/burdenrateledger-com-agentic-access.yml
summary_line: 9 operations · 7 acting
tags:
- Company
- Labor
- Calculator
- Small Business
---
