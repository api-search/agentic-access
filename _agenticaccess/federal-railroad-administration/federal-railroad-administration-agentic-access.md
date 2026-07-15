---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: federal-railroad-administration-openapi.yml
  format: yaml
  label: Federal Railroad Administration Public API
  slug: federal-railroad-administration
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-railroad-administration/refs/heads/main/openapi/federal-railroad-administration-openapi.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Federal Railroad Administration Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Federal Railroad Administration exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Federal Railroad Administration
provider_slug: federal-railroad-administration
slug: federal-railroad-administration-agentic-access
source_filename: federal-railroad-administration-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/federal-railroad-administration-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /accidents\n  method: get\n  operationId: listAccidents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /incidents\n  method: get\n  operationId: listIncidents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /crossings\n  method: get\n  operationId: listCrossings\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inspections\n  method: get\n  operationId: listInspections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operational-data\n  method: get\n  operationId: listOperationalData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/federal-railroad-administration/refs/heads/main/agentic-access/federal-railroad-administration-agentic-access.yml
summary_line: 5 operations
tags:
- Federal Government
- Railroads
- Safety
- Transportation
---
