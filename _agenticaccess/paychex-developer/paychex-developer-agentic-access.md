---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 4
api_specs:
- filename: paychex-payroll-companies-openapi.yml
  format: yaml
  label: Paychex Payroll Companies API
  slug: paychex-payroll-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paychex-developer/refs/heads/main/openapi/paychex-payroll-companies-openapi.yml
- filename: paychex-workers-openapi.yml
  format: yaml
  label: Paychex Workers API
  slug: paychex-workers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paychex-developer/refs/heads/main/openapi/paychex-workers-openapi.yml
- filename: paychex-time-openapi.yml
  format: yaml
  label: Paychex Time API
  slug: paychex-time-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paychex-developer/refs/heads/main/openapi/paychex-time-openapi.yml
consequence_counts:
  read: 4
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Paychex Developer Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Paychex exposes 5 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Paychex
provider_slug: paychex-developer
slug: paychex-developer-agentic-access
source_filename: paychex-developer-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/paychex-payroll-companies-openapi.yml, openapi/paychex-time-openapi.yml, openapi/paychex-workers-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 4\n    acting: 1\n  by_consequence:\n    read: 4\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /companies\n  method: get\n  operationId: listCompanies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyId}\n  method: get\n  operationId: getCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /time/v1/timeentries\n  method: post\n  operationId: createTimeEntries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{companyId}/workers\n  method: get\n  operationId: listCompanyWorkers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{companyId}/workers/{workerId}\n  method: get\n  operationId: getCompanyWorker\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paychex-developer/refs/heads/main/agentic-access/paychex-developer-agentic-access.yml
summary_line: 5 operations · 1 acting
tags:
- Benefits
- HCM
- HR
- Paychex Flex
- Payroll
- Time and Attendance
- Workforce
- Fortune 1000
---
