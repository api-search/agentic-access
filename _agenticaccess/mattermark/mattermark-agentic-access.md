---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 10
api_specs:
- filename: mattermark-companies-api-openapi.yml
  format: yaml
  label: Mattermark Companies API
  slug: mattermark-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mattermark/refs/heads/main/openapi/mattermark-companies-api-openapi.yml
- filename: mattermark-complex-queries-api-openapi.yml
  format: yaml
  label: Mattermark Complex Queries API
  slug: mattermark-complex-queries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mattermark/refs/heads/main/openapi/mattermark-complex-queries-api-openapi.yml
- filename: mattermark-funding-events-api-openapi.yml
  format: yaml
  label: Mattermark Funding Events API
  slug: mattermark-funding-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mattermark/refs/heads/main/openapi/mattermark-funding-events-api-openapi.yml
- filename: mattermark-investors-api-openapi.yml
  format: yaml
  label: Mattermark Investors API
  slug: mattermark-investors-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mattermark/refs/heads/main/openapi/mattermark-investors-api-openapi.yml
- filename: mattermark-search-api-openapi.yml
  format: yaml
  label: Mattermark Search API
  slug: mattermark-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mattermark/refs/heads/main/openapi/mattermark-search-api-openapi.yml
- filename: mattermark-utilities-api-openapi.yml
  format: yaml
  label: Mattermark Utilities API
  slug: mattermark-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mattermark/refs/heads/main/openapi/mattermark-utilities-api-openapi.yml
consequence_counts:
  read: 10
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Mattermark Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'Mattermark exposes 11 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Mattermark
provider_slug: mattermark
slug: mattermark-agentic-access
source_filename: mattermark-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: generated\nsource: openapi/mattermark-rest-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 10\n    acting: 1\n  by_consequence:\n    read: 10\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /search\n  method: get\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies\n  method: get\n  operationId: get_companies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{id}\n  method: get\n  operationId:\
  \ get_company\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{id}/stories\n  method: get\n  operationId: get_company_stories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{id}/similar\n  method: get\n  operationId: get_similar_companies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{id}/people\n  method: get\n  operationId: get_company_personnel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fundings\n  method: get\n  operationId: searchFunding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /investors/{id}\n  method: get\n  operationId: get_investor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /investors/{id}/portfolio\n  method: get\n  operationId: get_investor_portfolio\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /queries\n  method: post\n  operationId: query_investors\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ratelimit/usage\n  method: get\n  operationId: quota\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mattermark/refs/heads/main/agentic-access/mattermark-agentic-access.yml
summary_line: 11 operations · 1 acting
tags:
- Company
- Business Intelligence
- Company Data
- Investors
- Funding
- Sales Intelligence
- Market Research
---
