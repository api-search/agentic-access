---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 11
api_specs:
- filename: smarthr-openapi.yml
  format: yaml
  label: SmartHR Crews API
  slug: smarthr-crews-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarthr/refs/heads/main/openapi/smarthr-openapi.yml
- filename: smarthr-openapi.yml
  format: yaml
  label: SmartHR Departments API
  slug: smarthr-departments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarthr/refs/heads/main/openapi/smarthr-openapi.yml
- filename: smarthr-openapi.yml
  format: yaml
  label: SmartHR Employment Types API
  slug: smarthr-employment-types-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarthr/refs/heads/main/openapi/smarthr-openapi.yml
- filename: smarthr-openapi.yml
  format: yaml
  label: SmartHR Custom Field Templates API
  slug: smarthr-custom-field-templates-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarthr/refs/heads/main/openapi/smarthr-openapi.yml
- filename: smarthr-openapi.yml
  format: yaml
  label: SmartHR Business Establishments API
  slug: smarthr-business-establishments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarthr/refs/heads/main/openapi/smarthr-openapi.yml
- filename: smarthr-openapi.yml
  format: yaml
  label: SmartHR Webhooks API
  slug: smarthr-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/smarthr/refs/heads/main/openapi/smarthr-openapi.yml
consequence_counts:
  read: 11
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Smarthr Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 27
overview: 'SmartHR exposes 27 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read and 16 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: SmartHR
provider_slug: smarthr
slug: smarthr-agentic-access
source_filename: smarthr-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/smarthr-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    connected: 11\n    acting: 16\n  by_consequence:\n    read: 11\n    write: 16\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/crews\n  method: get\n  operationId: listCrews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/crews\n  method: post\n  operationId: createCrew\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/crews/{id}\n  method: get\n  operationId: getCrew\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/crews/{id}\n  method: patch\n  operationId: updateCrew\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/crews/{id}\n  method: delete\n  operationId: deleteCrew\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/crews/{id}/invite\n\
  \  method: put\n  operationId: inviteCrew\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/departments\n  method: get\n  operationId: listDepartments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/departments\n  method: post\n  operationId: createDepartment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/departments/{id}\n  method: get\n  operationId: getDepartment\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/departments/{id}\n  method: patch\n  operationId: updateDepartment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/departments/{id}\n  method: delete\n  operationId: deleteDepartment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/employment_types\n  method: get\n  operationId: listEmploymentTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/employment_types\n  method: post\n  operationId: createEmploymentType\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/employment_types/{id}\n  method: get\n  operationId: getEmploymentType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/employment_types/{id}\n  method: patch\n  operationId: updateEmploymentType\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/employment_types/{id}\n  method: delete\n  operationId: deleteEmploymentType\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/crew_custom_field_templates\n  method: get\n  operationId: listCrewCustomFieldTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/crew_custom_field_templates\n  method: post\n  operationId: createCrewCustomFieldTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v1/crew_custom_field_templates/{id}\n  method: get\n  operationId: getCrewCustomFieldTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/crew_custom_field_templates/{id}\n  method: patch\n  operationId: updateCrewCustomFieldTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/crew_custom_field_templates/{id}\n  method: delete\n  operationId: deleteCrewCustomFieldTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n   \
  \ audit: required\n- path: /v1/biz_establishments\n  method: get\n  operationId: listBizEstablishments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/{id}\n  method: get\n  operationId: getWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/webhooks/{id}\n  method: patch\n  operationId: updateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/{id}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/smarthr/refs/heads/main/agentic-access/smarthr-agentic-access.yml
summary_line: 27 operations · 16 acting
tags:
- HR
- Human Resources
- HRIS
- Labor Management
- Payroll
- Japan
- Employees
- Personnel
- Onboarding
- SaaS
---
