---
acting_count: 0
action_class_counts:
  connected: 7
api_specs:
- filename: centers-for-medicare-and-medicaid-services-cms-blue-button-2-openapi.yml
  format: yaml
  label: CMS Blue Button 2.0 API
  slug: cms-blue-button-2
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/centers-for-medicare-and-medicaid-services/refs/heads/main/openapi/centers-for-medicare-and-medicaid-services-cms-blue-button-2-openapi.yml
consequence_counts:
  read: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Centers For Medicare And Medicaid Services Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Centers for Medicare and Medicaid Services exposes 7 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Centers for Medicare and Medicaid Services
provider_slug: centers-for-medicare-and-medicaid-services
slug: centers-for-medicare-and-medicaid-services-agentic-access
source_filename: centers-for-medicare-and-medicaid-services-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/centers-for-medicare-and-medicaid-services-cms-blue-button-2-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 7\n  by_consequence:\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /metadata\n  method: get\n  operationId: getCapabilityStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Patient\n  method: get\n  operationId: searchPatient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Patient/{id}\n\
  \  method: get\n  operationId: readPatient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Coverage\n  method: get\n  operationId: searchCoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Coverage/{id}\n  method: get\n  operationId: readCoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ExplanationOfBenefit\n  method: get\n  operationId: searchExplanationOfBenefit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ExplanationOfBenefit/{id}\n  method: get\n  operationId: readExplanationOfBenefit\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/centers-for-medicare-and-medicaid-services/refs/heads/main/agentic-access/centers-for-medicare-and-medicaid-services-agentic-access.yml
summary_line: 7 operations
tags:
- BCDA
- Blue Button
- CMS
- Claims
- DPC
- FHIR
- Federal Government
- Healthcare
- Interoperability
- Marketplace
- Medicaid
- Medicare
- Open Data
- Provider Data
- Socrata
---
