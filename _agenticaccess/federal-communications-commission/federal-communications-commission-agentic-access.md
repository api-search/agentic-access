---
acting_count: 0
action_class_counts:
  connected: 4
api_specs:
- filename: federal-communications-commission-datasets-api-openapi.yml
  format: yaml
  label: Federal Communications Commission Datasets API
  slug: federal-communications-commission-datasets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-communications-commission/refs/heads/main/openapi/federal-communications-commission-datasets-api-openapi.yml
- filename: federal-communications-commission-filings-api-openapi.yml
  format: yaml
  label: Federal Communications Commission Filings API
  slug: federal-communications-commission-filings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-communications-commission/refs/heads/main/openapi/federal-communications-commission-filings-api-openapi.yml
- filename: federal-communications-commission-pirate-radio-api-openapi.yml
  format: yaml
  label: Federal Communications Commission Pirate Radio API
  slug: federal-communications-commission-pirate-radio-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-communications-commission/refs/heads/main/openapi/federal-communications-commission-pirate-radio-api-openapi.yml
- filename: federal-communications-commission-proceedings-api-openapi.yml
  format: yaml
  label: Federal Communications Commission Proceedings API
  slug: federal-communications-commission-proceedings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-communications-commission/refs/heads/main/openapi/federal-communications-commission-proceedings-api-openapi.yml
consequence_counts:
  read: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Federal Communications Commission Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'Federal Communications Commission exposes 4 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Federal Communications Commission
provider_slug: federal-communications-commission
slug: federal-communications-commission-agentic-access
source_filename: federal-communications-commission-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/ecfs.yml, openapi/opendata.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    connected: 4\n  by_consequence:\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /filings\n  method: get\n  operationId: listFilings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /proceedings\n  method: get\n  operationId: listProceedings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/views.json\n  method: get\n  operationId: listViews\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/wgq8-eb5c.json\n  method: get\n  operationId: listPirateRadio\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/federal-communications-commission/refs/heads/main/agentic-access/federal-communications-commission-agentic-access.yml
summary_line: 4 operations
tags:
- Communications
- Federal Government
- Open Data
---
