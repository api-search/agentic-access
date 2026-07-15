---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: nasdaq-omx-group-openapi.yml
  format: yaml
  label: Nasdaq Data Link Time-series API
  slug: data-link-time-series
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nasdaq-omx-group/refs/heads/main/openapi/nasdaq-omx-group-openapi.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Nasdaq Omx Group Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Nasdaq exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Nasdaq
provider_slug: nasdaq-omx-group
slug: nasdaq-omx-group-agentic-access
source_filename: nasdaq-omx-group-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/nasdaq-omx-group-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /datasets/{database_code}/{dataset_code}/data.{format}\n  method: get\n  operationId: getDatasetData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datasets/{database_code}/{dataset_code}/metadata.{format}\n  method: get\n  operationId: getDatasetMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /datasets/{database_code}/{dataset_code}.{format}\n  method: get\n  operationId: getDatasetDataAndMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /databases/{database_code}.{format}\n  method: get\n  operationId: getDatabaseMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /databases/{database_code}/data\n  method: get\n  operationId: downloadDatabaseData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nasdaq-omx-group/refs/heads/main/agentic-access/nasdaq-omx-group-agentic-access.yml
summary_line: 5 operations
tags:
- Financial Services
- Capital Markets
- Stock Exchange
- Market Data
- Economics
- Fortune 1000
---
