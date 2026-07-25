---
acting_count: 0
action_class_counts:
  connected: 8
api_specs:
- filename: obie-opendata-atm-locator-standard.json
  format: json
  label: Weatherbys Bank Open Data ATM Locator API
  slug: weatherbys-open-data-atm-locator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weatherbys-bank/refs/heads/main/openapi/obie-opendata-atm-locator-standard.json
- filename: obie-opendata-branch-locator-standard.json
  format: json
  label: Weatherbys Bank Open Data Branch Locator API
  slug: weatherbys-open-data-branch-locator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weatherbys-bank/refs/heads/main/openapi/obie-opendata-branch-locator-standard.json
- filename: obie-opendata-personal-current-accounts-standard.json
  format: json
  label: Weatherbys Bank Open Data Personal Current Accounts API
  slug: weatherbys-open-data-personal-current-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weatherbys-bank/refs/heads/main/openapi/obie-opendata-personal-current-accounts-standard.json
- filename: obie-opendata-business-current-accounts-standard.json
  format: json
  label: Weatherbys Bank Open Data Business Current Accounts API
  slug: weatherbys-open-data-business-current-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/weatherbys-bank/refs/heads/main/openapi/obie-opendata-business-current-accounts-standard.json
consequence_counts:
  read: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Weatherbys Bank Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Weatherbys Bank exposes 8 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Weatherbys Bank
provider_slug: weatherbys-bank
slug: weatherbys-bank-agentic-access
source_filename: weatherbys-bank-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: generated\nsource: openapi/obie-opendata-atm-locator-standard.json, openapi/obie-opendata-branch-locator-standard.json,\n  openapi/obie-opendata-business-current-accounts-standard.json, openapi/obie-opendata-personal-current-accounts-standard.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 8\n  by_consequence:\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /atms\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /atms\n  method: head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /branches\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /branches\n  method: head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /business-current-accounts\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /business-current-accounts\n  method: head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /personal-current-accounts\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /personal-current-accounts\n  method: head\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/weatherbys-bank/refs/heads/main/agentic-access/weatherbys-bank-agentic-access.yml
summary_line: 8 operations
tags:
- Financial Services
- Banking
- Open Banking
- PSD2
- OBIE
- United Kingdom
- Payments
- Account Information
- Private Banking
---
