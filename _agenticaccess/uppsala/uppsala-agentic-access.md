---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: uppsala-battledeaths-api-openapi.yml
  format: yaml
  label: Uppsala University BattleDeaths API
  slug: uppsala-battledeaths-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uppsala/refs/heads/main/openapi/uppsala-battledeaths-api-openapi.yml
- filename: uppsala-dyadic-api-openapi.yml
  format: yaml
  label: Uppsala University Dyadic API
  slug: uppsala-dyadic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uppsala/refs/heads/main/openapi/uppsala-dyadic-api-openapi.yml
- filename: uppsala-gedevents-api-openapi.yml
  format: yaml
  label: Uppsala University GEDEvents API
  slug: uppsala-gedevents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uppsala/refs/heads/main/openapi/uppsala-gedevents-api-openapi.yml
- filename: uppsala-nonstate-api-openapi.yml
  format: yaml
  label: Uppsala University NonState API
  slug: uppsala-nonstate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uppsala/refs/heads/main/openapi/uppsala-nonstate-api-openapi.yml
- filename: uppsala-onesided-api-openapi.yml
  format: yaml
  label: Uppsala University OneSided API
  slug: uppsala-onesided-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uppsala/refs/heads/main/openapi/uppsala-onesided-api-openapi.yml
- filename: uppsala-organizedviolencecy-api-openapi.yml
  format: yaml
  label: Uppsala University OrganizedViolenceCY API
  slug: uppsala-organizedviolencecy-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uppsala/refs/heads/main/openapi/uppsala-organizedviolencecy-api-openapi.yml
- filename: uppsala-ucdpprioconflict-api-openapi.yml
  format: yaml
  label: Uppsala University UcdpPrioConflict API
  slug: uppsala-ucdpprioconflict-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/uppsala/refs/heads/main/openapi/uppsala-ucdpprioconflict-api-openapi.yml
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Uppsala Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Uppsala University exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Uppsala University
provider_slug: uppsala
slug: uppsala-agentic-access
source_filename: uppsala-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/uppsala-ucdp.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /api/BattleDeaths/{version}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/Dyadic/{version}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/GEDEvents/{version}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/NonState/{version}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/OneSided/{version}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/organizedviolencecy/{version}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/UcdpPrioConflict/{version}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/uppsala/refs/heads/main/agentic-access/uppsala-agentic-access.yml
summary_line: 7 operations
tags:
- University
- Higher Education
- Education
- Sweden
- Public Research University
- Research Data
- Institutional Repository
- Identity Federation
- Research Computing
- Conflict Data
- Open Access
---
