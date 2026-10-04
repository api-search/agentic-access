---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 3
api_specs:
- filename: brainbase-apicontract-api-openapi.yml
  format: yaml
  label: Brainbase ApiContract API
  slug: brainbase-apicontract-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brainbase/refs/heads/main/openapi/brainbase-apicontract-api-openapi.yml
- filename: brainbase-general-api-openapi.yml
  format: yaml
  label: Brainbase General API
  slug: brainbase-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/brainbase/refs/heads/main/openapi/brainbase-general-api-openapi.yml
consequence_counts:
  read: 3
  safety-critical: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Brainbase Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/report/runtime/error
operation_count: 4
overview: 'Brainbase exposes 4 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Brainbase
provider_slug: brainbase
slug: brainbase-agentic-access
source_filename: brainbase-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/brainbase-apicontract-api-openapi.yml, openapi/brainbase-general-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    connected: 3\n    acting: 1\n  by_consequence:\n    read: 3\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /api/user/contracts\n  method: get\n  operationId: ApiContractController__userAssociatedContracts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/report/runtime/error\n  method: post\n  operationId: GeneralController__reportRuntimeError\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/get/information/general\n  method: post\n  operationId: GeneralController__getGeneralApplicationInformation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/get/information/git\n  method: get\n  operationId: GeneralController__getGitInformation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/brainbase/refs/heads/main/agentic-access/brainbase-agentic-access.yml
summary_line: 4 operations · 1 acting · 1 human-in-the-loop
tags:
- Company
- Cloud
- Intellectual Property
- Brand Licensing
- Licensing Management
- Royalties
- Contracts
- Trademarks
- Software-as-a-Service
---
