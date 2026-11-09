---
acting_count: 0
action_class_counts:
  connected: 16
api_specs:
- filename: bankday-dev-account-api-openapi.yml
  format: yaml
  label: bankday-dev Account API
  slug: bankday-dev-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bankday-dev/openapi/bankday-dev-account-api-openapi.yml
- filename: bankday-dev-ach-api-openapi.yml
  format: yaml
  label: bankday-dev Ach API
  slug: bankday-dev-ach-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bankday-dev/openapi/bankday-dev-ach-api-openapi.yml
- filename: bankday-dev-business-day-api-openapi.yml
  format: yaml
  label: bankday-dev Business Day API
  slug: bankday-dev-business-day-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bankday-dev/openapi/bankday-dev-business-day-api-openapi.yml
- filename: bankday-dev-business-days-api-openapi.yml
  format: yaml
  label: bankday-dev Business Days API
  slug: bankday-dev-business-days-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bankday-dev/openapi/bankday-dev-business-days-api-openapi.yml
- filename: bankday-dev-calendars-api-openapi.yml
  format: yaml
  label: bankday-dev Calendars API
  slug: bankday-dev-calendars-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bankday-dev/openapi/bankday-dev-calendars-api-openapi.yml
- filename: bankday-dev-fx-api-openapi.yml
  format: yaml
  label: bankday-dev Fx API
  slug: bankday-dev-fx-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bankday-dev/openapi/bankday-dev-fx-api-openapi.yml
- filename: bankday-dev-holidays-api-openapi.yml
  format: yaml
  label: bankday-dev Holidays API
  slug: bankday-dev-holidays-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bankday-dev/openapi/bankday-dev-holidays-api-openapi.yml
- filename: bankday-dev-minimum-wage-api-openapi.yml
  format: yaml
  label: bankday-dev Minimum Wage API
  slug: bankday-dev-minimum-wage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bankday-dev/openapi/bankday-dev-minimum-wage-api-openapi.yml
- filename: bankday-dev-payroll-api-openapi.yml
  format: yaml
  label: bankday-dev Payroll API
  slug: bankday-dev-payroll-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bankday-dev/openapi/bankday-dev-payroll-api-openapi.yml
- filename: bankday-dev-today-api-openapi.yml
  format: yaml
  label: bankday-dev Today API
  slug: bankday-dev-today-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bankday-dev/openapi/bankday-dev-today-api-openapi.yml
consequence_counts:
  read: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bankday Dev Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'bankday-dev exposes 16 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: bankday-dev
provider_slug: bankday-dev
slug: bankday-dev-agentic-access
source_filename: bankday-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/bankday-dev-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 16\n  by_consequence:\n    read: 16\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/business-day\n  method: get\n  operationId: business_day\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/today\n  method: get\n  operationId: today\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/business-days/add\n  method: get\n  operationId: add\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/business-days/count\n  method: get\n  operationId: count\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/business-days/next\n  method: get\n  operationId: next\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/business-days/roll\n  method: get\n  operationId: roll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/business-days\n  method: get\n  operationId: list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/holidays\n\
  \  method: get\n  operationId: holidays\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fx/spot\n  method: get\n  operationId: fx\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/ach/settlement\n  method: get\n  operationId: ach\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payroll/schedule\n  method: get\n  operationId: payroll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/calendars\n  method: get\n  operationId: calendars\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/minimum-wage\n  method: get\n  operationId: minimum_wage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/minimum-wage/changes\n  method: get\n  operationId: minimum_wage_changes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/minimum-wage/jurisdictions\n  method: get\n  operationId: minimum_wage_jurisdictions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/account\n  method: get\n  operationId: account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/bankday-dev/agentic-access/bankday-dev-agentic-access.yml
summary_line: 16 operations
tags:
- Company
- Finance
- Calendar
- Payments
---
