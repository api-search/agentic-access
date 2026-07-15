---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 13
api_specs:
- filename: flexpa-openapi.yml
  format: yaml
  label: Flexpa Link / Connect API
  slug: flexpa-link-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexpa/refs/heads/main/openapi/flexpa-openapi.yml
- filename: flexpa-openapi.yml
  format: yaml
  label: Flexpa Access Tokens API
  slug: flexpa-access-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexpa/refs/heads/main/openapi/flexpa-openapi.yml
- filename: flexpa-openapi.yml
  format: yaml
  label: Flexpa FHIR Resources API
  slug: flexpa-fhir-resources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexpa/refs/heads/main/openapi/flexpa-openapi.yml
- filename: flexpa-openapi.yml
  format: yaml
  label: Flexpa Claims Data API
  slug: flexpa-claims-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/flexpa/refs/heads/main/openapi/flexpa-openapi.yml
consequence_counts:
  read: 13
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Flexpa Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'Flexpa exposes 15 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Flexpa
provider_slug: flexpa
slug: flexpa-agentic-access
source_filename: flexpa-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/flexpa-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 13\n    acting: 2\n  by_consequence:\n    read: 13\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /oauth/authorize\n  method: get\n  operationId: authorize\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/token\n  method: post\n  operationId: token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /fhir/metadata\n  method: get\n  operationId: getCapabilityStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/Patient\n  method: get\n  operationId: searchPatient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/Patient/{id}\n  method: get\n  operationId: readPatient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/Patient/{id}/$everything\n  method: get\n  operationId: patientEverything\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/Patient/{id}/$summary\n\
  \  method: get\n  operationId: patientSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/Patient/{id}/$pdf\n  method: get\n  operationId: patientPdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/Coverage\n  method: get\n  operationId: searchCoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/Coverage/{id}\n  method: get\n  operationId: readCoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/ExplanationOfBenefit\n  method: get\n  operationId: searchExplanationOfBenefit\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/ExplanationOfBenefit/{id}\n  method: get\n  operationId: readExplanationOfBenefit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/Practitioner\n  method: get\n  operationId: searchPractitioner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/Organization\n  method: get\n  operationId: searchOrganization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fhir/ViewDefinition/$run\n  method: post\n  operationId: runViewDefinition\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/flexpa/refs/heads/main/agentic-access/flexpa-agentic-access.yml
summary_line: 15 operations · 2 acting
tags:
- Healthcare
- FHIR
- Patient Access
- Claims Data
- Health Insurance
---
