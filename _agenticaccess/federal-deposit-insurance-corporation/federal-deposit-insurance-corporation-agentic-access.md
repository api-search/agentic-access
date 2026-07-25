---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: federal-deposit-insurance-corporation-demographics-api-openapi.yml
  format: yaml
  label: Federal Deposit Insurance Corporation Demographics API
  slug: federal-deposit-insurance-corporation-demographics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-deposit-insurance-corporation/refs/heads/main/openapi/federal-deposit-insurance-corporation-demographics-api-openapi.yml
- filename: federal-deposit-insurance-corporation-deposits-api-openapi.yml
  format: yaml
  label: Federal Deposit Insurance Corporation Deposits API
  slug: federal-deposit-insurance-corporation-deposits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-deposit-insurance-corporation/refs/heads/main/openapi/federal-deposit-insurance-corporation-deposits-api-openapi.yml
- filename: federal-deposit-insurance-corporation-failures-api-openapi.yml
  format: yaml
  label: Federal Deposit Insurance Corporation Failures API
  slug: federal-deposit-insurance-corporation-failures-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-deposit-insurance-corporation/refs/heads/main/openapi/federal-deposit-insurance-corporation-failures-api-openapi.yml
- filename: federal-deposit-insurance-corporation-financials-api-openapi.yml
  format: yaml
  label: Federal Deposit Insurance Corporation Financials API
  slug: federal-deposit-insurance-corporation-financials-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-deposit-insurance-corporation/refs/heads/main/openapi/federal-deposit-insurance-corporation-financials-api-openapi.yml
- filename: federal-deposit-insurance-corporation-history-api-openapi.yml
  format: yaml
  label: Federal Deposit Insurance Corporation History API
  slug: federal-deposit-insurance-corporation-history-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-deposit-insurance-corporation/refs/heads/main/openapi/federal-deposit-insurance-corporation-history-api-openapi.yml
- filename: federal-deposit-insurance-corporation-institutions-api-openapi.yml
  format: yaml
  label: Federal Deposit Insurance Corporation Institutions API
  slug: federal-deposit-insurance-corporation-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-deposit-insurance-corporation/refs/heads/main/openapi/federal-deposit-insurance-corporation-institutions-api-openapi.yml
- filename: federal-deposit-insurance-corporation-locations-api-openapi.yml
  format: yaml
  label: Federal Deposit Insurance Corporation Locations API
  slug: federal-deposit-insurance-corporation-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/federal-deposit-insurance-corporation/refs/heads/main/openapi/federal-deposit-insurance-corporation-locations-api-openapi.yml
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Federal Deposit Insurance Corporation Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Federal Deposit Insurance Corporation exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Federal Deposit Insurance Corporation
provider_slug: federal-deposit-insurance-corporation
slug: federal-deposit-insurance-corporation-agentic-access
source_filename: federal-deposit-insurance-corporation-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/bankfind.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /institutions\n  method: get\n  operationId: listInstitutions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locations\n  method: get\n  operationId: listLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /financials\n  method: get\n  operationId: listFinancials\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /history\n  method: get\n  operationId: listHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /failures\n  method: get\n  operationId: listFailures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sod\n  method: get\n  operationId: listSummaryOfDeposits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /demographics\n  method: get\n  operationId: listDemographics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/federal-deposit-insurance-corporation/refs/heads/main/agentic-access/federal-deposit-insurance-corporation-agentic-access.yml
summary_line: 7 operations
tags:
- Banking
- Federal Government
- Financial Data
- Insurance
---
