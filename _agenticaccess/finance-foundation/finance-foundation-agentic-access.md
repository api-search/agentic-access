---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 24
api_specs:
- filename: finance-foundation-all-api-openapi.yml
  format: yaml
  label: finance-foundation All API
  slug: finance-foundation-all-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finance-foundation/openapi/finance-foundation-all-api-openapi.yml
- filename: finance-foundation-assets-api-openapi.yml
  format: yaml
  label: finance-foundation Assets API
  slug: finance-foundation-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finance-foundation/openapi/finance-foundation-assets-api-openapi.yml
- filename: finance-foundation-banks-api-openapi.yml
  format: yaml
  label: finance-foundation Banks API
  slug: finance-foundation-banks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finance-foundation/openapi/finance-foundation-banks-api-openapi.yml
- filename: finance-foundation-clearing-api-openapi.yml
  format: yaml
  label: finance-foundation Clearing API
  slug: finance-foundation-clearing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finance-foundation/openapi/finance-foundation-clearing-api-openapi.yml
- filename: finance-foundation-companies-api-openapi.yml
  format: yaml
  label: finance-foundation Companies API
  slug: finance-foundation-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finance-foundation/openapi/finance-foundation-companies-api-openapi.yml
- filename: finance-foundation-countries-api-openapi.yml
  format: yaml
  label: finance-foundation Countries API
  slug: finance-foundation-countries-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finance-foundation/openapi/finance-foundation-countries-api-openapi.yml
- filename: finance-foundation-finance-foundation-api-api-openapi.yml
  format: yaml
  label: finance-foundation Finance Foundation API
  slug: finance-foundation-finance-foundation-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finance-foundation/openapi/finance-foundation-finance-foundation-api-api-openapi.yml
- filename: finance-foundation-funds-api-openapi.yml
  format: yaml
  label: finance-foundation Funds API
  slug: finance-foundation-funds-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finance-foundation/openapi/finance-foundation-funds-api-openapi.yml
- filename: finance-foundation-graph-api-openapi.yml
  format: yaml
  label: finance-foundation Graph API
  slug: finance-foundation-graph-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finance-foundation/openapi/finance-foundation-graph-api-openapi.yml
- filename: finance-foundation-indicators-api-openapi.yml
  format: yaml
  label: finance-foundation Indicators API
  slug: finance-foundation-indicators-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finance-foundation/openapi/finance-foundation-indicators-api-openapi.yml
- filename: finance-foundation-ingest-api-openapi.yml
  format: yaml
  label: finance-foundation Ingest API
  slug: finance-foundation-ingest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finance-foundation/openapi/finance-foundation-ingest-api-openapi.yml
- filename: finance-foundation-live-api-openapi.yml
  format: yaml
  label: finance-foundation Live API
  slug: finance-foundation-live-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finance-foundation/openapi/finance-foundation-live-api-openapi.yml
- filename: finance-foundation-markets-api-openapi.yml
  format: yaml
  label: finance-foundation Markets API
  slug: finance-foundation-markets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finance-foundation/openapi/finance-foundation-markets-api-openapi.yml
- filename: finance-foundation-research-api-openapi.yml
  format: yaml
  label: finance-foundation Research API
  slug: finance-foundation-research-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finance-foundation/openapi/finance-foundation-research-api-openapi.yml
- filename: finance-foundation-resolve-api-openapi.yml
  format: yaml
  label: finance-foundation Resolve API
  slug: finance-foundation-resolve-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finance-foundation/openapi/finance-foundation-resolve-api-openapi.yml
- filename: finance-foundation-schema-api-openapi.yml
  format: yaml
  label: finance-foundation Schema API
  slug: finance-foundation-schema-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finance-foundation/openapi/finance-foundation-schema-api-openapi.yml
- filename: finance-foundation-search-api-openapi.yml
  format: yaml
  label: finance-foundation Search API
  slug: finance-foundation-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/finance-foundation/openapi/finance-foundation-search-api-openapi.yml
consequence_counts:
  physical: 1
  read: 24
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Finance Foundation Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/ingest
operation_count: 25
overview: 'finance-foundation exposes 25 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 read and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: finance-foundation
provider_slug: finance-foundation
slug: finance-foundation-agentic-access
source_filename: finance-foundation-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/finance-foundation-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 25\n  by_action_class:\n    connected: 24\n    acting: 1\n  by_consequence:\n    read: 24\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/all\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/schema\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/indicators\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/search\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/resolve\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/ingest\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /api/v1/live\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/graph/{type}/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/companies\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/companies/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/markets\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/markets/{id}\n  method: get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/assets\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/assets/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/funds\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/funds/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/banks\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/banks/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/countries\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/countries/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/research\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/research/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/v1/clearing\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/clearing/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/finance-foundation/agentic-access/finance-foundation-agentic-access.yml
summary_line: 25 operations · 1 acting
tags:
- Finance
- Data
- Open Data
- Artificial Intelligence
---
