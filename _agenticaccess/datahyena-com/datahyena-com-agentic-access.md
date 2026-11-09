---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 8
api_specs:
- filename: datahyena-com-acquisitions-api-openapi.yml
  format: yaml
  label: datahyena-com Acquisitions API
  slug: datahyena-com-acquisitions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datahyena-com/openapi/datahyena-com-acquisitions-api-openapi.yml
- filename: datahyena-com-companies-api-openapi.yml
  format: yaml
  label: datahyena-com Companies API
  slug: datahyena-com-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datahyena-com/openapi/datahyena-com-companies-api-openapi.yml
- filename: datahyena-com-exec-moves-api-openapi.yml
  format: yaml
  label: datahyena-com Exec Moves API
  slug: datahyena-com-exec-moves-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datahyena-com/openapi/datahyena-com-exec-moves-api-openapi.yml
- filename: datahyena-com-funding-events-api-openapi.yml
  format: yaml
  label: datahyena-com Funding Events API
  slug: datahyena-com-funding-events-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datahyena-com/openapi/datahyena-com-funding-events-api-openapi.yml
- filename: datahyena-com-hiring-signals-api-openapi.yml
  format: yaml
  label: datahyena-com Hiring Signals API
  slug: datahyena-com-hiring-signals-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datahyena-com/openapi/datahyena-com-hiring-signals-api-openapi.yml
- filename: datahyena-com-investors-api-openapi.yml
  format: yaml
  label: datahyena-com Investors API
  slug: datahyena-com-investors-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/datahyena-com/openapi/datahyena-com-investors-api-openapi.yml
consequence_counts:
  read: 8
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Datahyena Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'datahyena-com exposes 10 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: datahyena-com
provider_slug: datahyena-com
slug: datahyena-com-agentic-access
source_filename: datahyena-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/datahyena-com.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 8\n    acting: 2\n  by_consequence:\n    read: 8\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/funding-events\n  method: get\n  operationId: funding_events_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/acquisitions\n  method: get\n  operationId: acquisitions_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/exec-moves\n  method:\
  \ get\n  operationId: exec_moves_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/hiring-signals\n  method: get\n  operationId: hiring_signals_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies\n  method: get\n  operationId: companies_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/timeline\n  method: get\n  operationId: company_timeline_single\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/timeline\n  method: post\n  operationId: company_timeline_bulk\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/companies/hiring\n  method: get\n  operationId: company_hiring_single\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/companies/hiring\n  method: post\n  operationId: company_hiring_bulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/investors\n  method: get\n  operationId: investors_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n"
source_yaml_url: https://artifacts.apis.io/datahyena-com/agentic-access/datahyena-com-agentic-access.yml
summary_line: 10 operations · 2 acting
tags:
- Company
- Data
- Funding
- M&A
- Hiring
---
