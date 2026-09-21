---
acting_count: 0
action_class_counts:
  connected: 4
api_specs:
- filename: ingest0r-com-openapi.yml
  format: yaml
  label: Cook County (Chicago) Property Records API
  slug: cook-county-property-records-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ingest0r-com/refs/heads/main/openapi/ingest0r-com-openapi.yml
consequence_counts:
  read: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ingest0R Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'ingest0r exposes 4 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ingest0r
provider_slug: ingest0r-com
slug: ingest0r-com-agentic-access
source_filename: ingest0r-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: generated\nsource: openapi/ingest0r-com-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    connected: 4\n  by_consequence:\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/search/{q}\n  method: get\n  operationId: v1_search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/parcel/{pin}\n  method: get\n  operationId: v1_parcel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/dossier/{pin}\n  method: get\n  operationId: v1_dossier\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/comps/{pin}\n  method: get\n  operationId: v1_comps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ingest0r-com/refs/heads/main/agentic-access/ingest0r-com-agentic-access.yml
summary_line: 4 operations
tags:
- Company
- Real-Estate
- Property Records
- Property Data
- Public Records
- Open Data
- Government Data
- Parcel
- Geocoding
- Property Tax
- Building Permits
- Comparable Sales
- Valuation
- x402
- Agentic Commerce
- MCP
- A2A
- agent-native
- Chicago
- Illinois
---
