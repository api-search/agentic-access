---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 2
api_specs:
- filename: moxe-health-chart-retrieval-initiate-openapi.json
  format: json
  label: Moxe Health Chart Retrieval API
  slug: moxe-health-chart-retrieval-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moxe-health/refs/heads/main/openapi/moxe-health-chart-retrieval-initiate-openapi.json
- filename: moxe-health-claim-management-initiate-openapi.json
  format: json
  label: Moxe Health Claim Management API
  slug: moxe-health-claim-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moxe-health/refs/heads/main/openapi/moxe-health-claim-management-initiate-openapi.json
consequence_counts:
  read: 2
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Moxe Health Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'Moxe Health exposes 4 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Moxe Health
provider_slug: moxe-health
slug: moxe-health-agentic-access
source_filename: moxe-health-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: generated\nsource: openapi/moxe-health-chart-retrieval-initiate-openapi.json, openapi/moxe-health-chart-retrieval-status-openapi.json,\n  openapi/moxe-health-claim-management-initiate-openapi.json, openapi/moxe-health-claim-management-status-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    acting: 2\n    connected: 2\n  by_consequence:\n    write: 2\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/patient-chart-request\n  method: post\n  operationId: initiateChartRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:patient-chart-request\n    audience: null\n    token:\n     \
  \ max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/patient-chart-request/{moxeRequestId}/status\n  method: get\n  operationId: getChartRequestStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:patient-chart-request\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/claim-management-request\n  method: post\n  operationId: initiateClaimManagementRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - write:claim-management-request\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/claim-management-request/{moxeRequestId}/status\n  method: get\n  operationId: getClaimManagementRequestStatus\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read:claim-management-request\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moxe-health/refs/heads/main/agentic-access/moxe-health-agentic-access.yml
summary_line: 4 operations · 2 acting
tags:
- Healthcare
- United States
- Interoperability
- Clinical Data
- Payer
- Provider
- EHR
- Health Data Exchange
- Claims
- Risk Adjustment
---
