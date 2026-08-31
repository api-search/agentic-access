---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 5
api_specs:
- filename: legal-ge-public-apis-directory-api-openapi.yml
  format: yaml
  label: legal.ge Public APIs Directory API
  slug: legal-ge-public-apis-directory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/legal-ge-public-apis/refs/heads/main/openapi/legal-ge-public-apis-directory-api-openapi.yml
- filename: legal-ge-public-apis-matching-api-openapi.yml
  format: yaml
  label: legal.ge Public APIs Matching API
  slug: legal-ge-public-apis-matching-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/legal-ge-public-apis/refs/heads/main/openapi/legal-ge-public-apis-matching-api-openapi.yml
consequence_counts:
  read: 5
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Legal Ge Public Apis Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'legal.ge Public APIs exposes 6 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: legal.ge Public APIs
provider_slug: legal-ge-public-apis
slug: legal-ge-public-apis-agentic-access
source_filename: legal-ge-public-apis-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: generated\nsource: openapi/legal-ge-public-apis-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 1\n    connected: 5\n  by_consequence:\n    write: 1\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /api/ask\n  method: post\n  operationId: askMatchSpecialists\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/ask\n  method: get\n  operationId: askMatchSpecialistsGet\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ask/classify\n  method: get\n  operationId: classifyLegalIntent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/service-search\n  method: get\n  operationId: searchServicesAndCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/specialists/search\n  method: get\n  operationId: searchSpecialistsByName\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/specialists/{id}/contact\n  method: get\n  operationId: revealSpecialistContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/legal-ge-public-apis/refs/heads/main/agentic-access/legal-ge-public-apis-agentic-access.yml
summary_line: 6 operations · 1 acting
tags:
- Legal
- law
- legal-services
- Directory
- georgia
- AI Agents
- MCP
- specialists
- professional-services
- Marketplace
- multilingual
- legal-tech
---
