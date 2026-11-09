---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 4
api_specs:
- filename: crivum-org-avaliacoes-api-openapi.yml
  format: yaml
  label: Crivum Avaliacoes API
  slug: crivum-org-avaliacoes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crivum-org/openapi/crivum-org-avaliacoes-api-openapi.yml
- filename: crivum-org-criterios-api-openapi.yml
  format: yaml
  label: Crivum Criterios API
  slug: crivum-org-criterios-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crivum-org/openapi/crivum-org-criterios-api-openapi.yml
- filename: crivum-org-records-api-openapi.yml
  format: yaml
  label: Crivum Records API
  slug: crivum-org-records-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crivum-org/openapi/crivum-org-records-api-openapi.yml
- filename: crivum-org-saldo-api-openapi.yml
  format: yaml
  label: Crivum Saldo API
  slug: crivum-org-saldo-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crivum-org/openapi/crivum-org-saldo-api-openapi.yml
- filename: crivum-org-triagem-api-openapi.yml
  format: yaml
  label: Crivum Triagem API
  slug: crivum-org-triagem-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/crivum-org/openapi/crivum-org-triagem-api-openapi.yml
consequence_counts:
  read: 4
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Crivum Org Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Crivum exposes 6 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Crivum
provider_slug: crivum-org
slug: crivum-org-agentic-access
source_filename: crivum-org-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/crivum-org-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 2\n    connected: 4\n  by_consequence:\n    write: 2\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/avaliacoes\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/avaliacoes/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /v1/saldo\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/triagem\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/criterios\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/records\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/crivum-org/agentic-access/crivum-org-agentic-access.yml
summary_line: 6 operations · 2 acting
tags:
- Platform
- Evaluation
- Publishing
- Artificial Intelligence
- Portuguese
---
