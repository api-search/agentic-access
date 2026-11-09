---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 9
api_specs:
- filename: firmastat-cz-firma-api-openapi.yml
  format: yaml
  label: Firmastat Firma API
  slug: firmastat-cz-firma-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmastat-cz/openapi/firmastat-cz-firma-api-openapi.yml
- filename: firmastat-cz-firmy-api-openapi.yml
  format: yaml
  label: Firmastat Firmy API
  slug: firmastat-cz-firmy-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmastat-cz/openapi/firmastat-cz-firmy-api-openapi.yml
- filename: firmastat-cz-health-api-openapi.yml
  format: yaml
  label: Firmastat Health API
  slug: firmastat-cz-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmastat-cz/openapi/firmastat-cz-health-api-openapi.yml
- filename: firmastat-cz-osoba-api-openapi.yml
  format: yaml
  label: Firmastat Osoba API
  slug: firmastat-cz-osoba-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmastat-cz/openapi/firmastat-cz-osoba-api-openapi.yml
- filename: firmastat-cz-osoby-api-openapi.yml
  format: yaml
  label: Firmastat Osoby API
  slug: firmastat-cz-osoby-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmastat-cz/openapi/firmastat-cz-osoby-api-openapi.yml
- filename: firmastat-cz-suggest-api-openapi.yml
  format: yaml
  label: Firmastat Suggest API
  slug: firmastat-cz-suggest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmastat-cz/openapi/firmastat-cz-suggest-api-openapi.yml
- filename: firmastat-cz-vyhledavani-api-openapi.yml
  format: yaml
  label: Firmastat Vyhledavani API
  slug: firmastat-cz-vyhledavani-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/firmastat-cz/openapi/firmastat-cz-vyhledavani-api-openapi.yml
consequence_counts:
  read: 9
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Firmastat Cz Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Firmastat exposes 10 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Firmastat
provider_slug: firmastat-cz
slug: firmastat-cz-agentic-access
source_filename: firmastat-cz-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-08'\nmethod: generated\nsource: openapi/firmastat-cz-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 9\n    acting: 1\n  by_consequence:\n    read: 9\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/vyhledavani\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/vyhledavani/export\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/firma/{ico}\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/firmy/dph\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/firma/{ico}/export\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/firma/{ico}/finance\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/osoby\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/v1/osoba/{klic}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/suggest\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/health\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/firmastat-cz/agentic-access/firmastat-cz-agentic-access.yml
summary_line: 10 operations · 1 acting
tags:
- Company
- API
- Czech
- Business
- Data
- Search
---
