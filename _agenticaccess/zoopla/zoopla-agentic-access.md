---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 6
api_specs:
- filename: zoopla-products-api-openapi.yml
  format: yaml
  label: Zoopla Products API
  slug: zoopla-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoopla/refs/heads/main/openapi/zoopla-products-api-openapi.yml
- filename: zoopla-rest-endpoints-api-openapi.yml
  format: yaml
  label: Zoopla REST Endpoints API
  slug: zoopla-rest-endpoints-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zoopla/refs/heads/main/openapi/zoopla-rest-endpoints-api-openapi.yml
consequence_counts:
  read: 6
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Zoopla Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Zoopla exposes 9 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Zoopla
provider_slug: zoopla
slug: zoopla-agentic-access
source_filename: zoopla-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-26'\nmethod: generated\nsource: openapi/zoopla-leads-api-openapi.json, openapi/zoopla-premium-listing-activations-openapi.json,\n  openapi/zoopla-weekly-featured-property-activations-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 6\n    acting: 3\n  by_consequence:\n    read: 6\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /applicant-leads\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - leads/list:applicant-leads\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /appraisal-leads\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    scope:\n    - leads/list:appraisal-leads\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /products/premium-listings/{uuid}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - api/api_access\n- path: /products/premium-listings/{uuid}\n  method: patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - api/api_access\n- path: /products/premium-listings\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - api/api_access\n- path: /products/premium-listings\n\
  \  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - api/api_access\n- path: /products/weekly-featured-properties/{uuid}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - api/api_access\n- path: /products/weekly-featured-properties\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - api/api_access\n- path: /products/weekly-featured-properties\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - api/api_access\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zoopla/refs/heads/main/agentic-access/zoopla-agentic-access.yml
summary_line: 9 operations · 3 acting
tags:
- Real-Estate
- United Kingdom
- Property Listings
- Property Portal
- PropTech
- Rentals
- Estate Agents
- Leads
- CRM Integration
---
