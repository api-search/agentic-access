---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 10
api_specs:
- filename: knight-frank-cmspage-api-openapi.yml
  format: yaml
  label: Knight Frank CMS Page API
  slug: knight-frank-cmspage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knight-frank/refs/heads/main/openapi/knight-frank-cmspage-api-openapi.yml
- filename: knight-frank-intelligencelab-api-openapi.yml
  format: yaml
  label: Knight Frank Intelligence Lab API
  slug: knight-frank-intelligencelab-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knight-frank/refs/heads/main/openapi/knight-frank-intelligencelab-api-openapi.yml
- filename: knight-frank-office-api-openapi.yml
  format: yaml
  label: Knight Frank Office API
  slug: knight-frank-office-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knight-frank/refs/heads/main/openapi/knight-frank-office-api-openapi.yml
- filename: knight-frank-person-api-openapi.yml
  format: yaml
  label: Knight Frank Person API
  slug: knight-frank-person-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knight-frank/refs/heads/main/openapi/knight-frank-person-api-openapi.yml
- filename: knight-frank-search-api-openapi.yml
  format: yaml
  label: Knight Frank Search API
  slug: knight-frank-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knight-frank/refs/heads/main/openapi/knight-frank-search-api-openapi.yml
- filename: knight-frank-serviceline-api-openapi.yml
  format: yaml
  label: Knight Frank Service Line API
  slug: knight-frank-serviceline-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knight-frank/refs/heads/main/openapi/knight-frank-serviceline-api-openapi.yml
- filename: knight-frank-telemetry-api-openapi.yml
  format: yaml
  label: Knight Frank Telemetry API
  slug: knight-frank-telemetry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/knight-frank/refs/heads/main/openapi/knight-frank-telemetry-api-openapi.yml
consequence_counts:
  read: 10
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Knight Frank Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'Knight Frank exposes 11 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Knight Frank
provider_slug: knight-frank
slug: knight-frank-agentic-access
source_filename: knight-frank-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: generated\nsource: openapi/knight-frank-api-v3-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 10\n    acting: 1\n  by_consequence:\n    read: 10\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /cmspage\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /intelligencelab\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /intelligencelab/facets\n  method: get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /office\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /office/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /person\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /person/autocomplete\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /person/cms-search\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /search\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /service-lines\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /telemetry/increment-selected-count\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/knight-frank/refs/heads/main/agentic-access/knight-frank-agentic-access.yml
summary_line: 11 operations · 1 acting
tags:
- Real-Estate
- United Kingdom
- Property Listings
- Commercial Real Estate
- Valuation
- Brokerage
- Property Management
- Rentals
- PropTech
- Research
---
