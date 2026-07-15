---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 8
api_specs:
- filename: nmbrs-openapi.yml
  format: yaml
  label: Nmbrs Companies API
  slug: nmbrs-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nmbrs/refs/heads/main/openapi/nmbrs-openapi.yml
- filename: nmbrs-openapi.yml
  format: yaml
  label: Nmbrs Employees API
  slug: nmbrs-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nmbrs/refs/heads/main/openapi/nmbrs-openapi.yml
- filename: nmbrs-openapi.yml
  format: yaml
  label: Nmbrs Employments API
  slug: nmbrs-employments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nmbrs/refs/heads/main/openapi/nmbrs-openapi.yml
- filename: nmbrs-openapi.yml
  format: yaml
  label: Nmbrs Payroll & Payruns API
  slug: nmbrs-payroll-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nmbrs/refs/heads/main/openapi/nmbrs-openapi.yml
- filename: nmbrs-openapi.yml
  format: yaml
  label: Nmbrs Wage Components API
  slug: nmbrs-wage-components-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nmbrs/refs/heads/main/openapi/nmbrs-openapi.yml
- filename: nmbrs-openapi.yml
  format: yaml
  label: Nmbrs Absences API
  slug: nmbrs-absences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/nmbrs/refs/heads/main/openapi/nmbrs-openapi.yml
consequence_counts:
  read: 8
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Nmbrs Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Nmbrs exposes 10 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Nmbrs
provider_slug: nmbrs
slug: nmbrs-agentic-access
source_filename: nmbrs-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/nmbrs-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 8\n    acting: 2\n  by_consequence:\n    read: 8\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/companies\n  method: get\n  operationId: listCompanies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/companies/{companyId}/employees\n  method: get\n  operationId: listCompanyEmployees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/employees/{employeeId}\n\
  \  method: get\n  operationId: getEmployee\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/employees/{employeeId}/employments\n  method: get\n  operationId: listEmployments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/employees/{employeeId}/salaries\n  method: get\n  operationId: listSalaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/employees/{employeeId}/wagecomponents\n  method: get\n  operationId: listWageComponents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/employees/{employeeId}/wagecomponents\n  method: post\n  operationId: createWageComponent\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/companies/{companyId}/payruns\n  method: get\n  operationId: listPayruns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/employees/{employeeId}/absences\n  method: get\n  operationId: listAbsences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/employees/{employeeId}/absences\n  method: post\n  operationId: createAbsence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/nmbrs/refs/heads/main/agentic-access/nmbrs-agentic-access.yml
summary_line: 10 operations · 2 acting
tags:
- Human Resources
- HRIS
- Payroll
- Employee Management
- HR
- Absence Management
- Netherlands
- Sweden
- SOAP
- REST
---
