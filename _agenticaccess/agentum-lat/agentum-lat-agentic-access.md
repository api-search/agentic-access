---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 6
api_specs:
- filename: agentum-lat-apis-brasil-openapi.json
  format: json
  label: AGENTUM APIs Brasil
  slug: apis-brasil
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentum-lat/refs/heads/main/openapi/agentum-lat-apis-brasil-openapi.json
- filename: agentum-lat-business-openapi.json
  format: json
  label: AGENTUM Business API
  slug: business
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/agentum-lat/refs/heads/main/openapi/agentum-lat-business-openapi.json
consequence_counts:
  read: 6
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Agentum Lat Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'AGENTUM exposes 7 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AGENTUM
provider_slug: agentum-lat
slug: agentum-lat-agentic-access
source_filename: agentum-lat-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-19'\nmethod: generated\nsource: openapi/agentum-lat-apis-brasil-openapi.json, openapi/agentum-lat-business-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    acting: 1\n    connected: 6\n  by_consequence:\n    write: 1\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /business-intelligence\n  method: post\n  operationId: businessIntelligence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verificar-cnpj\n  method: get\n  operationId:\
  \ verificarCnpj\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /verificar-cep\n  method: get\n  operationId: verificarCep\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /taxas-brasil\n  method: get\n  operationId: taxasBrasil\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /preflight\n  method: get\n  operationId: preflight\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company-intelligence\n  method: get\n  operationId: companyIntelligence\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /company\n  method: get\n  operationId: company\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/agentum-lat/refs/heads/main/agentic-access/agentum-lat-agentic-access.yml
summary_line: 7 operations · 1 acting
tags:
- Company
- Business Intelligence
- KYB
- Company Data
- Compliance
- Brazil
- x402
- Agentic Commerce
- Exchange Rates
- Address Verification
- Economic Data
- MCP
- A2A
- Agents
---
