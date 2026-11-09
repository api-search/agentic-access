---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 13
api_specs:
- filename: dhamma-gift-mcp-api-openapi.yml
  format: yaml
  label: Dhamma.Gift MCP API
  slug: dhamma-gift-mcp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dhamma-gift/openapi/dhamma-gift-mcp-api-openapi.yml
- filename: dhamma-gift-search-api-openapi.yml
  format: yaml
  label: Dhamma.Gift Search API
  slug: dhamma-gift-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dhamma-gift/openapi/dhamma-gift-search-api-openapi.yml
- filename: dhamma-gift-text-api-openapi.yml
  format: yaml
  label: Dhamma.Gift Text API
  slug: dhamma-gift-text-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dhamma-gift/openapi/dhamma-gift-text-api-openapi.yml
- filename: dhamma-gift-toc-api-openapi.yml
  format: yaml
  label: Dhamma.Gift Toc API
  slug: dhamma-gift-toc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dhamma-gift/openapi/dhamma-gift-toc-api-openapi.yml
- filename: dhamma-gift-tts-api-openapi.yml
  format: yaml
  label: Dhamma.Gift Tts API
  slug: dhamma-gift-tts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dhamma-gift/openapi/dhamma-gift-tts-api-openapi.yml
- filename: dhamma-gift-uposatha-api-openapi.yml
  format: yaml
  label: Dhamma.Gift Uposatha API
  slug: dhamma-gift-uposatha-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dhamma-gift/openapi/dhamma-gift-uposatha-api-openapi.yml
consequence_counts:
  read: 13
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dhamma Gift Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'Dhamma.Gift exposes 16 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 13 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Dhamma.Gift
provider_slug: dhamma-gift
slug: dhamma-gift-agentic-access
source_filename: dhamma-gift-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/dhamma-gift-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 13\n    acting: 3\n  by_consequence:\n    read: 13\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /search\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/{keyword}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/enrich\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/text/{suttaId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/nav/{suttaId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/toc\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/toc/book/{code}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/transliterate\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/patimokkha-fragment/{side}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/tts/pali\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tts/memo\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/tts/dg-voices\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/tts/health\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mcp\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uposatha.ics\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/ai-search\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/dhamma-gift/agentic-access/dhamma-gift-agentic-access.yml
summary_line: 16 operations · 3 acting
tags:
- Buddhism
- Pali Canon
- Texts
- Search
- Audio
---
