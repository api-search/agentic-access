---
acting_count: 0
action_class_counts:
  connected: 6
api_specs:
- filename: verisk-catastrophe-api-openapi.yml
  format: yaml
  label: Verisk Catastrophe API
  slug: verisk-catastrophe-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verisk/refs/heads/main/openapi/verisk-catastrophe-api-openapi.yml
- filename: verisk-claims-api-openapi.yml
  format: yaml
  label: Verisk Claims API
  slug: verisk-claims-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verisk/refs/heads/main/openapi/verisk-claims-api-openapi.yml
- filename: verisk-property-api-openapi.yml
  format: yaml
  label: Verisk Property API
  slug: verisk-property-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verisk/refs/heads/main/openapi/verisk-property-api-openapi.yml
- filename: verisk-risk-scoring-api-openapi.yml
  format: yaml
  label: Verisk Risk Scoring API
  slug: verisk-risk-scoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/verisk/refs/heads/main/openapi/verisk-risk-scoring-api-openapi.yml
consequence_counts:
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Verisk Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Verisk exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Verisk
provider_slug: verisk
slug: verisk-agentic-access
source_filename: verisk-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/verisk-catastrophe-api-openapi.yml, openapi/verisk-claims-api-openapi.yml, openapi/verisk-property-api-openapi.yml,\n  openapi/verisk-risk-scoring-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 6\n  by_consequence:\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /catastrophe/peril-scores\n  method: post\n  operationId: getPerilScores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /claims/benchmarks\n  method: get\n  operationId: getClaimsBenchmarks\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /property/risk/{propertyId}\n  method: get\n  operationId: getPropertyRisk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /property/lookup\n  method: post\n  operationId: lookupPropertyByAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /risk/scores\n  method: post\n  operationId: getRiskScores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /risk/fire-protection-class\n  method: get\n  operationId: getFireProtectionClass\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/verisk/refs/heads/main/agentic-access/verisk-agentic-access.yml
summary_line: 6 operations
tags:
- Insurance
- Analytics
- Risk Management
- Property Data
- Catastrophe Modeling
- Underwriting
- Claims
---
