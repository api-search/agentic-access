---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: wadifa-info-agenda-api-openapi.yml
  format: yaml
  label: Wadifa Info Agenda API
  slug: wadifa-info-agenda-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wadifa-info/refs/heads/main/openapi/wadifa-info-agenda-api-openapi.yml
- filename: wadifa-info-concours-api-openapi.yml
  format: yaml
  label: Wadifa Info Concours API
  slug: wadifa-info-concours-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wadifa-info/refs/heads/main/openapi/wadifa-info-concours-api-openapi.yml
- filename: wadifa-info-jours-feries-api-openapi.yml
  format: yaml
  label: Wadifa Info Jours Feries API
  slug: wadifa-info-jours-feries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wadifa-info/refs/heads/main/openapi/wadifa-info-jours-feries-api-openapi.yml
- filename: wadifa-info-salaires-api-openapi.yml
  format: yaml
  label: Wadifa Info Salaires API
  slug: wadifa-info-salaires-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wadifa-info/refs/heads/main/openapi/wadifa-info-salaires-api-openapi.yml
- filename: wadifa-info-vacances-scolaires-api-openapi.yml
  format: yaml
  label: Wadifa Info Vacances Scolaires API
  slug: wadifa-info-vacances-scolaires-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wadifa-info/refs/heads/main/openapi/wadifa-info-vacances-scolaires-api-openapi.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Wadifa Info Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Wadifa Info exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Wadifa Info
provider_slug: wadifa-info
slug: wadifa-info-agentic-access
source_filename: wadifa-info-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: generated\nsource: openapi/wadifa-info-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/concours\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/salaires\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agenda/dates-limites\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/jours-feries\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/vacances-scolaires\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wadifa-info/refs/heads/main/agentic-access/wadifa-info-agentic-access.yml
summary_line: 5 operations
tags:
- Company
- Jobs
- Public Sector
- Morocco
- Open Data
- Salaries
- Government
---
