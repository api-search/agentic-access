---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: university-of-cape-town-catalog-api-openapi.yml
  format: yaml
  label: DataFirst Microdata Catalog API (NADA)
  slug: datafirst-nada
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/university-of-cape-town/refs/heads/main/openapi/university-of-cape-town-catalog-api-openapi.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: derived
name: University Of Cape Town Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'University of Cape Town exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: University of Cape Town
provider_slug: university-of-cape-town
slug: university-of-cape-town-agentic-access
source_filename: university-of-cape-town-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-30'\nmethod: derived\nsource: openapi/_original/university-of-cape-town-datafirst-nada.yaml\nx-operator: institution\nnote: Figshare operations (articles/collections/projects) were REMOVED on 2026-08-30 — they belong to\n  Figshare's contract behind UCT's ZivaHub tenancy, not to UCT. Every remaining operation is an unauthenticated\n  read on UCT's own DataFirst host.\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI.\n  A governance starting point for exposing this API to AI agents — review and bind audience per deployment.\n  See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /catalog\n  method: get\n  operationId: listCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n   \
  \ audit: none\n- path: /catalog/search\n  method: get\n  operationId: searchCatalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/{idno}\n  method: get\n  operationId: getStudy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/data_files/{idno}\n  method: get\n  operationId: listStudyDataFiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /catalog/variables/{idno}\n  method: get\n  operationId: listStudyVariables\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/university-of-cape-town/refs/heads/main/agentic-access/university-of-cape-town-agentic-access.yml
summary_line: 5 operations
tags:
- University
- Higher Education
- Education
- Public Research University
- South Africa
- Africa
- Research Data
- Open Data
- Institutional Repository
- OAI-PMH
- Identity Federation
- Microdata
- Research Computing
---
