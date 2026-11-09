---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 10
api_specs:
- filename: steamgpt-net-bans-api-openapi.yml
  format: yaml
  label: steamgpt-net Bans API
  slug: steamgpt-net-bans-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/steamgpt-net/openapi/steamgpt-net-bans-api-openapi.yml
- filename: steamgpt-net-batch-api-openapi.yml
  format: yaml
  label: steamgpt-net Batch API
  slug: steamgpt-net-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/steamgpt-net/openapi/steamgpt-net-batch-api-openapi.yml
- filename: steamgpt-net-compare-api-openapi.yml
  format: yaml
  label: steamgpt-net Compare API
  slug: steamgpt-net-compare-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/steamgpt-net/openapi/steamgpt-net-compare-api-openapi.yml
- filename: steamgpt-net-converter-api-openapi.yml
  format: yaml
  label: steamgpt-net Converter API
  slug: steamgpt-net-converter-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/steamgpt-net/openapi/steamgpt-net-converter-api-openapi.yml
- filename: steamgpt-net-faceit-api-openapi.yml
  format: yaml
  label: steamgpt-net Faceit API
  slug: steamgpt-net-faceit-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/steamgpt-net/openapi/steamgpt-net-faceit-api-openapi.yml
- filename: steamgpt-net-friends-api-openapi.yml
  format: yaml
  label: steamgpt-net Friends API
  slug: steamgpt-net-friends-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/steamgpt-net/openapi/steamgpt-net-friends-api-openapi.yml
- filename: steamgpt-net-identity-api-openapi.yml
  format: yaml
  label: steamgpt-net Identity API
  slug: steamgpt-net-identity-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/steamgpt-net/openapi/steamgpt-net-identity-api-openapi.yml
- filename: steamgpt-net-profile-api-openapi.yml
  format: yaml
  label: steamgpt-net Profile API
  slug: steamgpt-net-profile-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/steamgpt-net/openapi/steamgpt-net-profile-api-openapi.yml
- filename: steamgpt-net-ready-api-openapi.yml
  format: yaml
  label: steamgpt-net Ready API
  slug: steamgpt-net-ready-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/steamgpt-net/openapi/steamgpt-net-ready-api-openapi.yml
- filename: steamgpt-net-summary-api-openapi.yml
  format: yaml
  label: steamgpt-net Summary API
  slug: steamgpt-net-summary-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/steamgpt-net/openapi/steamgpt-net-summary-api-openapi.yml
consequence_counts:
  read: 10
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Steamgpt Net Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'steamgpt-net exposes 11 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: steamgpt-net
provider_slug: steamgpt-net
slug: steamgpt-net-agentic-access
source_filename: steamgpt-net-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/steamgpt-net-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 10\n    acting: 1\n  by_consequence:\n    read: 10\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /summary/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - rate-boost\n- path: /profile/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - rate-boost\n- path: /friends/{id}\n  method: get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - rate-boost\n- path: /faceit/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - rate-boost\n- path: /batch/{ids}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - rate-boost\n- path: /converter/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - rate-boost\n- path: /identity/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  \    scope:\n    - rate-boost\n- path: /bans/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - rate-boost\n- path: /compare/{id1}/{id2}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - rate-boost\n- path: /batch\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - rate-boost\n- path: /ready\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - rate-boost\n"
source_yaml_url: https://artifacts.apis.io/steamgpt-net/agentic-access/steamgpt-net-agentic-access.yml
summary_line: 11 operations · 1 acting
tags:
- Company
- Artificial Intelligence
- Gaming
- Steam
---
