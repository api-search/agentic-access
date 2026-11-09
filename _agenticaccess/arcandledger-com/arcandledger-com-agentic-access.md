---
acting_count: 0
action_class_counts:
  connected: 11
api_specs:
- filename: arcandledger-com-deadlines-api-openapi.yml
  format: yaml
  label: arcandledger-com Deadlines API
  slug: arcandledger-com-deadlines-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcandledger-com/openapi/arcandledger-com-deadlines-api-openapi.yml
- filename: arcandledger-com-interest-rates-api-openapi.yml
  format: yaml
  label: arcandledger-com Interest Rates API
  slug: arcandledger-com-interest-rates-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcandledger-com/openapi/arcandledger-com-interest-rates-api-openapi.yml
- filename: arcandledger-com-notices-api-openapi.yml
  format: yaml
  label: arcandledger-com Notices API
  slug: arcandledger-com-notices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcandledger-com/openapi/arcandledger-com-notices-api-openapi.yml
- filename: arcandledger-com-openapi-json-api-openapi.yml
  format: yaml
  label: arcandledger-com Openapi.json API
  slug: arcandledger-com-openapi-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcandledger-com/openapi/arcandledger-com-openapi-json-api-openapi.yml
- filename: arcandledger-com-tax-documents-api-openapi.yml
  format: yaml
  label: arcandledger-com Tax Documents API
  slug: arcandledger-com-tax-documents-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcandledger-com/openapi/arcandledger-com-tax-documents-api-openapi.yml
- filename: arcandledger-com-tax-parameters-api-openapi.yml
  format: yaml
  label: arcandledger-com Tax Parameters API
  slug: arcandledger-com-tax-parameters-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcandledger-com/openapi/arcandledger-com-tax-parameters-api-openapi.yml
- filename: arcandledger-com-vintages-api-openapi.yml
  format: yaml
  label: arcandledger-com Vintages API
  slug: arcandledger-com-vintages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/arcandledger-com/openapi/arcandledger-com-vintages-api-openapi.yml
consequence_counts:
  read: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Arcandledger Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'arcandledger-com exposes 11 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: arcandledger-com
provider_slug: arcandledger-com
slug: arcandledger-com-agentic-access
source_filename: arcandledger-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/arcandledger-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 11\n  by_consequence:\n    read: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/tax-parameters\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tax-parameters/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/deadlines\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/deadlines/estimated-payments\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/interest-rates\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/notices\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/notices/{code}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tax-documents\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/tax-documents/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vintages\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/openapi.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/arcandledger-com/agentic-access/arcandledger-com-agentic-access.yml
summary_line: 11 operations
tags:
- Accounting
- Tax
- Bookkeeping
- Financial Services
- Los Angeles
---
