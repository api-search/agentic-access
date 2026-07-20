---
acting_count: 0
action_class_counts:
  connected: 6
api_specs:
- filename: collectors-psa-openapi-original.json
  format: json
  label: PSA Public API
  slug: psa-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/collectors/refs/heads/main/openapi/collectors-psa-openapi-original.json
consequence_counts:
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Collectors Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Collectors exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Collectors
provider_slug: collectors
slug: collectors-agentic-access
source_filename: collectors-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/collectors-psa-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 6\n  by_consequence:\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /cert/GetByCertNumber/{certNumber}\n  method: get\n  operationId: Cert_GetByCertNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cert/GetByCertNumberForFileAppend/{certNumber}\n  method: get\n  operationId: Cert_GetByCertNumberForFileAppend\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /cert/GetImagesByCertNumber/{certNumber}\n  method: get\n  operationId: Cert_GetImagesByCertNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /order/GetProgress/{orderNumber}\n  method: get\n  operationId: Order_GetProgress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /order/GetSubmissionProgress/{submissionNumber}\n  method: get\n  operationId: Order_GetSubmissionProgress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pop/GetPSASpecPopulation/{specID}\n  method: get\n  operationId: Pop_GetPSASpecPopulation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/collectors/refs/heads/main/agentic-access/collectors-agentic-access.yml
summary_line: 6 operations
tags:
- Company
- Marketplace
- Collectibles
- Authentication
- Grading
- Trading Cards
- Verification
---
