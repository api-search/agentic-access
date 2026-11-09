---
acting_count: 0
action_class_counts:
  connected: 12
api_specs:
- filename: datocapital-com-account-api-openapi.yml
  format: yaml
  label: Dato Capital Account API
  slug: datocapital-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datocapital-com/openapi/datocapital-com-account-api-openapi.yml
- filename: datocapital-com-companies-api-openapi.yml
  format: yaml
  label: Dato Capital Companies API
  slug: datocapital-com-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datocapital-com/openapi/datocapital-com-companies-api-openapi.yml
- filename: datocapital-com-filings-api-openapi.yml
  format: yaml
  label: Dato Capital Filings API
  slug: datocapital-com-filings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datocapital-com/openapi/datocapital-com-filings-api-openapi.yml
- filename: datocapital-com-health-api-openapi.yml
  format: yaml
  label: Dato Capital Health API
  slug: datocapital-com-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datocapital-com/openapi/datocapital-com-health-api-openapi.yml
- filename: datocapital-com-individuals-api-openapi.yml
  format: yaml
  label: Dato Capital Individuals API
  slug: datocapital-com-individuals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datocapital-com/openapi/datocapital-com-individuals-api-openapi.yml
- filename: datocapital-com-reference-api-openapi.yml
  format: yaml
  label: Dato Capital Reference API
  slug: datocapital-com-reference-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datocapital-com/openapi/datocapital-com-reference-api-openapi.yml
- filename: datocapital-com-suggest-api-openapi.yml
  format: yaml
  label: Dato Capital Suggest API
  slug: datocapital-com-suggest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datocapital-com/openapi/datocapital-com-suggest-api-openapi.yml
consequence_counts:
  read: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Datocapital Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Dato Capital exposes 12 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Dato Capital
provider_slug: datocapital-com
slug: datocapital-com-agentic-access
source_filename: datocapital-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/datocapital-com-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 12\n  by_consequence:\n    read: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /v3/health\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/ready\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/whoami\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/reference/countries\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/companies\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/companies/{uec}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/companies/{uec}/filings\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/companies/{uec}/representatives\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v3/{country}/{company_number}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/individuals\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/individuals/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/suggest\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/datocapital-com/agentic-access/datocapital-com-agentic-access.yml
summary_line: 12 operations
tags:
- Company
- Data
- Search
- Compliance
- Due Diligence
---
