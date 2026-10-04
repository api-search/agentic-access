---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 6
api_specs:
- filename: emitwise-facilities-api-openapi.yml
  format: yaml
  label: Emitwise Facilities API
  slug: emitwise-facilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emitwise/refs/heads/main/openapi/emitwise-facilities-api-openapi.yml
- filename: emitwise-files-api-openapi.yml
  format: yaml
  label: Emitwise Files API
  slug: emitwise-files-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emitwise/refs/heads/main/openapi/emitwise-files-api-openapi.yml
- filename: emitwise-projects-api-openapi.yml
  format: yaml
  label: Emitwise Projects API
  slug: emitwise-projects-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emitwise/refs/heads/main/openapi/emitwise-projects-api-openapi.yml
- filename: emitwise-schema-api-openapi.yml
  format: yaml
  label: Emitwise Schema API
  slug: emitwise-schema-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emitwise/refs/heads/main/openapi/emitwise-schema-api-openapi.yml
- filename: emitwise-suppliers-api-openapi.yml
  format: yaml
  label: Emitwise Suppliers API
  slug: emitwise-suppliers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/emitwise/refs/heads/main/openapi/emitwise-suppliers-api-openapi.yml
consequence_counts:
  read: 6
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Emitwise Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Emitwise exposes 7 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Emitwise
provider_slug: emitwise
slug: emitwise-agentic-access
source_filename: emitwise-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/emitwise-facilities-api-openapi.yml, openapi/emitwise-files-api-openapi.yml,\n  openapi/emitwise-projects-api-openapi.yml, openapi/emitwise-schema-api-openapi.yml, openapi/emitwise-suppliers-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 6\n    acting: 1\n  by_consequence:\n    read: 6\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /facilities\n  method: get\n  operationId: listFacilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files\n  method: post\n  operationId: uploadFile\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /files\n  method: get\n  operationId: listFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/{fileId}\n  method: get\n  operationId: getFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /projects\n  method: get\n  operationId: listProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schema\n  method: get\n  operationId: getSchema\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /suppliers/list\n  method: post\n  operationId: listSuppliers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/emitwise/refs/heads/main/agentic-access/emitwise-agentic-access.yml
summary_line: 7 operations · 1 acting
tags:
- Carbon Accounting
- Greenhouse Gas
- Scope 3
- Supply Chain Emissions
- Product Carbon Footprint
- Sustainability
- ESG
- CDP
- CSRD
- GHG Protocol
- Climate
- Procurement
- Artificial Intelligence
---
