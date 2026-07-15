---
acting_count: 10
action_class_counts:
  acting: 10
  connected: 10
api_specs:
- filename: workmotion-openapi.yml
  format: yaml
  label: WorkMotion Employees API
  slug: workmotion-employees-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workmotion/refs/heads/main/openapi/workmotion-openapi.yml
- filename: workmotion-openapi.yml
  format: yaml
  label: WorkMotion Contracts API
  slug: workmotion-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workmotion/refs/heads/main/openapi/workmotion-openapi.yml
- filename: workmotion-openapi.yml
  format: yaml
  label: WorkMotion Onboarding API
  slug: workmotion-onboarding-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workmotion/refs/heads/main/openapi/workmotion-openapi.yml
- filename: workmotion-openapi.yml
  format: yaml
  label: WorkMotion Absences API
  slug: workmotion-absences-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workmotion/refs/heads/main/openapi/workmotion-openapi.yml
- filename: workmotion-openapi.yml
  format: yaml
  label: WorkMotion Documents API
  slug: workmotion-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workmotion/refs/heads/main/openapi/workmotion-openapi.yml
- filename: workmotion-openapi.yml
  format: yaml
  label: WorkMotion Cost Calculator API
  slug: workmotion-cost-calculator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workmotion/refs/heads/main/openapi/workmotion-openapi.yml
- filename: workmotion-openapi.yml
  format: yaml
  label: WorkMotion Webhooks API
  slug: workmotion-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/workmotion/refs/heads/main/openapi/workmotion-openapi.yml
consequence_counts:
  read: 10
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Workmotion Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 20
overview: 'WorkMotion exposes 20 API operations that an AI agent could call, of which 10 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 10 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: WorkMotion
provider_slug: workmotion
slug: workmotion-agentic-access
source_filename: workmotion-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/workmotion-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 10\n    acting: 10\n  by_consequence:\n    read: 10\n    write: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /employees\n  method: get\n  operationId: listEmployees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employees\n  method: post\n  operationId: createEmployee\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employees/{employeeId}\n  method: get\n  operationId: getEmployee\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employees/{employeeId}\n  method: patch\n  operationId: updateEmployee\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /employees/{employeeId}/contracts\n  method: get\n  operationId: listEmployeeContracts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employees/{employeeId}/contracts\n  method: post\n  operationId: createContract\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contracts/{contractId}\n  method: get\n  operationId: getContract\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contracts/{contractId}\n  method: patch\n  operationId: updateContract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /onboardings\n  method: post\n  operationId: startOnboarding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /onboardings/{onboardingId}\n  method: get\n  operationId: getOnboarding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /absences\n  method: get\n  operationId: listAbsences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /absences\n  method: post\n  operationId: createAbsence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /absences/{absenceId}\n  method:\
  \ get\n  operationId: getAbsence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employees/{employeeId}/documents\n  method: get\n  operationId: listDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /employees/{employeeId}/documents\n  method: post\n  operationId: uploadDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{documentId}\n  method: get\n  operationId: downloadDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /cost-calculator\n  method: post\n  operationId: calculateEmploymentCost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{webhookId}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/workmotion/refs/heads/main/agentic-access/workmotion-agentic-access.yml
summary_line: 20 operations · 10 acting
tags:
- Employer of Record
- EOR
- Global Employment
- HR
- Payroll
- Onboarding
- Contractors
- Compliance
---
