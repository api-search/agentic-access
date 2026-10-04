---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 7
api_specs:
- filename: finch-auth-api-openapi.yml
  format: yaml
  label: Finch Auth API
  slug: finch-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finch/refs/heads/main/openapi/finch-auth-api-openapi.yml
- filename: finch-connect-api-openapi.yml
  format: yaml
  label: Finch Connect API
  slug: finch-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finch/refs/heads/main/openapi/finch-connect-api-openapi.yml
- filename: finch-employer-api-openapi.yml
  format: yaml
  label: Finch Employer API
  slug: finch-employer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/finch/refs/heads/main/openapi/finch-employer-api-openapi.yml
consequence_counts:
  read: 7
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Finch Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Finch exposes 9 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Finch
provider_slug: finch
slug: finch-agentic-access
source_filename: finch-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/finch-auth-api-openapi.yml, openapi/finch-connect-api-openapi.yml, openapi/finch-employer-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    acting: 2\n    connected: 7\n  by_consequence:\n    write: 2\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /auth/token\n  method: post\n  operationId: exchangeAuthCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connect/sessions\n  method: post\n\
  \  operationId: createConnectSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employer/company\n  method: get\n  operationId: getCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employer/directory\n  method: get\n  operationId: listDirectory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employer/individual\n  method: post\n  operationId: getIndividuals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employer/employment\n\
  \  method: post\n  operationId: getEmployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employer/payment\n  method: get\n  operationId: listPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employer/pay-statement\n  method: post\n  operationId: getPayStatements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employer/benefits\n  method: get\n  operationId: listBenefits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/finch/refs/heads/main/agentic-access/finch-agentic-access.yml
summary_line: 9 operations · 2 acting
tags:
- Employment
- HRIS
- Payroll
- Benefits
- Human Resources
- Unified API
- Workforce
- Integration
---
