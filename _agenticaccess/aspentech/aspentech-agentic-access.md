---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 2
api_specs:
- filename: aspentech-data-api-openapi.yml
  format: yaml
  label: AspenTech Data API
  slug: aspentech-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aspentech/refs/heads/main/openapi/aspentech-data-api-openapi.yml
- filename: aspentech-historical-api-openapi.yml
  format: yaml
  label: AspenTech Historical API
  slug: aspentech-historical-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aspentech/refs/heads/main/openapi/aspentech-historical-api-openapi.yml
- filename: aspentech-items-api-openapi.yml
  format: yaml
  label: AspenTech Items API
  slug: aspentech-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aspentech/refs/heads/main/openapi/aspentech-items-api-openapi.yml
- filename: aspentech-system-api-openapi.yml
  format: yaml
  label: AspenTech System API
  slug: aspentech-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/aspentech/refs/heads/main/openapi/aspentech-system-api-openapi.yml
consequence_counts:
  read: 2
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Aspentech Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'AspenTech exposes 6 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AspenTech
provider_slug: aspentech
slug: aspentech-agentic-access
source_filename: aspentech-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/aspentech-data-api-openapi.yml, openapi/aspentech-historical-api-openapi.yml,\n  openapi/aspentech-items-api-openapi.yml, openapi/aspentech-system-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 4\n    connected: 2\n  by_consequence:\n    write: 4\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api\n  method: post\n  operationId: executeRpcCall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api/data/read\n  method: post\n  operationId: readDataItems\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/data/write\n  method: post\n  operationId: writeDataItems\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/data/readhistory\n  method: post\n  operationId: readHistoricalData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n   \
  \   - abnormal\n      - high-value\n    audit: required\n- path: /api/item/get\n  method: post\n  operationId: getConfigurationItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/sys/info\n  method: get\n  operationId: getSystemInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/aspentech/refs/heads/main/agentic-access/aspentech-agentic-access.yml
summary_line: 6 operations · 4 acting
tags:
- Industrial IoT
- Process Optimization
- Manufacturing
- Energy
- Chemicals
- Time Series
---
