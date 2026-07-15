---
acting_count: 0
action_class_counts:
  connected: 8
api_specs:
- filename: cms-blue-button-openapi.yml
  format: yaml
  label: CMS Blue Button 2.0 Explanation of Benefit API
  slug: cms-blue-button-explanation-of-benefit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-blue-button/refs/heads/main/openapi/cms-blue-button-openapi.yml
- filename: cms-blue-button-openapi.yml
  format: yaml
  label: CMS Blue Button 2.0 Patient API
  slug: cms-blue-button-patient-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-blue-button/refs/heads/main/openapi/cms-blue-button-openapi.yml
- filename: cms-blue-button-openapi.yml
  format: yaml
  label: CMS Blue Button 2.0 Coverage API
  slug: cms-blue-button-coverage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-blue-button/refs/heads/main/openapi/cms-blue-button-openapi.yml
- filename: cms-blue-button-openapi.yml
  format: yaml
  label: CMS Blue Button 2.0 Authorization and UserInfo API
  slug: cms-blue-button-authorization-userinfo-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cms-blue-button/refs/heads/main/openapi/cms-blue-button-openapi.yml
consequence_counts:
  read: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cms Blue Button Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'CMS Blue Button 2.0 exposes 8 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CMS Blue Button 2.0
provider_slug: cms-blue-button
slug: cms-blue-button-agentic-access
source_filename: cms-blue-button-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cms-blue-button-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 8\n  by_consequence:\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /ExplanationOfBenefit\n  method: get\n  operationId: searchExplanationOfBenefit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - patient/Coverage.read\n    - patient/ExplanationOfBenefit.read\n    - patient/Patient.read\n- path: /ExplanationOfBenefit/{id}\n  method: get\n  operationId: readExplanationOfBenefit\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - patient/Coverage.read\n    - patient/ExplanationOfBenefit.read\n    - patient/Patient.read\n- path: /Patient\n  method: get\n  operationId: searchPatient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - patient/Coverage.read\n    - patient/ExplanationOfBenefit.read\n    - patient/Patient.read\n- path: /Patient/{id}\n  method: get\n  operationId: readPatient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - patient/Coverage.read\n    - patient/ExplanationOfBenefit.read\n    - patient/Patient.read\n- path: /Coverage\n  method: get\n  operationId: searchCoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n    scope:\n    - patient/Coverage.read\n    - patient/ExplanationOfBenefit.read\n    - patient/Patient.read\n- path: /Coverage/{id}\n  method: get\n  operationId: readCoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - patient/Coverage.read\n    - patient/ExplanationOfBenefit.read\n    - patient/Patient.read\n- path: /metadata\n  method: get\n  operationId: getCapabilityStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - patient/Coverage.read\n    - patient/ExplanationOfBenefit.read\n    - patient/Patient.read\n- path: /connect/userinfo\n  method: get\n  operationId: getUserInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n    scope:\n    - patient/Coverage.read\n    - patient/ExplanationOfBenefit.read\n    - patient/Patient.read\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cms-blue-button/refs/heads/main/agentic-access/cms-blue-button-agentic-access.yml
summary_line: 8 operations
tags:
- Blue Button
- CARIN
- Medicare
- FHIR
- Claims Data
- Patient Access
- Healthcare
- Government
---
