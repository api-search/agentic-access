---
acting_count: 0
action_class_counts:
  connected: 15
api_specs:
- filename: cajusticewatch-com-cajusticewatch-api-openapi.yml
  format: yaml
  label: CA Justice Watch Cajusticewatch API
  slug: cajusticewatch-com-cajusticewatch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cajusticewatch-com/openapi/cajusticewatch-com-cajusticewatch-api-openapi.yml
consequence_counts:
  read: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cajusticewatch Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 15
overview: 'CA Justice Watch exposes 15 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 15 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CA Justice Watch
provider_slug: cajusticewatch-com
slug: cajusticewatch-com-agentic-access
source_filename: cajusticewatch-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/cajusticewatch-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 15\n  by_consequence:\n    read: 15\n  human_in_the_loop_required: 0\noperations:\n- path: /api/rest/search_das\n  method: get\n  operationId: search_das\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rest/get_da\n  method: get\n  operationId: get_da\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rest/search_defenders\n  method: get\n  operationId:\
  \ search_defenders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rest/get_defender\n  method: get\n  operationId: get_defender\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rest/search_judges\n  method: get\n  operationId: search_judges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rest/search_officers\n  method: get\n  operationId: search_officers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rest/get_officer\n  method: get\n  operationId: get_officer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rest/search_cjp\n  method: get\n  operationId: search_cjp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rest/search_cjp_documents\n  method: get\n  operationId: search_cjp_documents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rest/search_capost\n  method: get\n  operationId: search_capost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rest/list_databases\n  method: get\n  operationId: list_databases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rest/top_das\n  method:\
  \ get\n  operationId: top_das\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rest/top_judges\n  method: get\n  operationId: top_judges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rest/top_officers\n  method: get\n  operationId: top_officers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/rest/list_pages\n  method: get\n  operationId: list_pages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/cajusticewatch-com/agentic-access/cajusticewatch-com-agentic-access.yml
summary_line: 15 operations
tags:
- Justice
- Transparency
- Data
- California
- Public Records
---
