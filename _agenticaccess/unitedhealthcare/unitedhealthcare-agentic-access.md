---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 7
api_specs:
- filename: unitedhealthcare-provider-api-openapi.yml
  format: yaml
  label: UnitedHealthcare Provider API
  slug: provider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unitedhealthcare/refs/heads/main/openapi/unitedhealthcare-provider-api-openapi.yml
- filename: unitedhealthcare-interoperability-api-openapi.yml
  format: yaml
  label: UnitedHealthcare Interoperability API
  slug: interoperability-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unitedhealthcare/refs/heads/main/openapi/unitedhealthcare-interoperability-api-openapi.yml
consequence_counts:
  read: 7
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Unitedhealthcare Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'UnitedHealthcare exposes 12 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: UnitedHealthcare
provider_slug: unitedhealthcare
slug: unitedhealthcare-agentic-access
source_filename: unitedhealthcare-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/unitedhealthcare-interoperability-api-openapi.yml, openapi/unitedhealthcare-provider-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 7\n    acting: 5\n  by_consequence:\n    read: 7\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /Patient/{id}\n  method: get\n  operationId: getPatient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ExplanationOfBenefit\n  method: get\n  operationId: listExplanationOfBenefit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /Coverage\n  method: get\n  operationId: listCoverage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Practitioner\n  method: get\n  operationId: listPractitioners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /Organization\n  method: get\n  operationId: listOrganizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /MedicationKnowledge\n  method: get\n  operationId: listFormulary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /eligibility/v1/real-time\n  method: post\n  operationId: checkEligibility\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /eligibility/v1/patient-benefit-check\n  method: post\n  operationId: checkPatientBenefit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claims/v1/pre-check\n  method: post\n  operationId: claimPreCheck\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /claims/v1/inquiry\n  method: post\n  operationId: inquireClaim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /prior-auth/v1/check\n  method: post\n  operationId: checkPriorAuth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /providers/v1/demographics\n  method: get\n  operationId: getProviderDemographics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unitedhealthcare/refs/heads/main/agentic-access/unitedhealthcare-agentic-access.yml
summary_line: 12 operations · 5 acting
tags:
- Health Insurance
- Healthcare
- FHIR
- Claims
- Eligibility
---
