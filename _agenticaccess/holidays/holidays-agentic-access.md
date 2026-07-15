---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: holidays-api-openapi.yml
  format: yaml
  label: Holiday API — Holidays
  slug: holidays
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/holidays/refs/heads/main/openapi/holidays-api-openapi.yml
- filename: holidays-api-openapi.yml
  format: yaml
  label: Holiday API — Countries
  slug: countries
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/holidays/refs/heads/main/openapi/holidays-api-openapi.yml
- filename: holidays-api-openapi.yml
  format: yaml
  label: Holiday API — Languages
  slug: languages
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/holidays/refs/heads/main/openapi/holidays-api-openapi.yml
- filename: holidays-api-openapi.yml
  format: yaml
  label: Holiday API — Workdays
  slug: workdays
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/holidays/refs/heads/main/openapi/holidays-api-openapi.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Holidays Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Holiday API exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Holiday API
provider_slug: holidays
slug: holidays-agentic-access
source_filename: holidays-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/holidays-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/holidays\n  method: get\n  operationId: listHolidays\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/countries\n  method: get\n  operationId: listCountries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/languages\n  method: get\n  operationId: listLanguages\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workday\n  method: get\n  operationId: getWorkday\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/workdays\n  method: get\n  operationId: getWorkdays\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/holidays/refs/heads/main/agentic-access/holidays-agentic-access.yml
summary_line: 5 operations
tags:
- Calendar
- Holidays
- Public Holidays
- Observances
- Reference Data
- Countries
- Languages
- Workdays
- Business Days
- Localization
---
