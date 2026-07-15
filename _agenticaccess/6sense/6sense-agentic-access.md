---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 2
api_specs:
- filename: 6sense-company-identification-api-openapi.yml
  format: yaml
  label: 6sense Company Identification API
  slug: 6sense-company-identification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/6sense/refs/heads/main/openapi/6sense-company-identification-api-openapi.yml
- filename: 6sense-company-firmographics-api-openapi.yml
  format: yaml
  label: 6sense Company Firmographics API
  slug: 6sense-company-firmographics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/6sense/refs/heads/main/openapi/6sense-company-firmographics-api-openapi.yml
- filename: 6sense-lead-scoring-api-openapi.yml
  format: yaml
  label: 6sense Lead Scoring API
  slug: 6sense-lead-scoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/6sense/refs/heads/main/openapi/6sense-lead-scoring-api-openapi.yml
- filename: 6sense-lead-scoring-firmographics-api-openapi.yml
  format: yaml
  label: 6sense Lead Scoring And Firmographics API
  slug: 6sense-lead-scoring-firmographics-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/6sense/refs/heads/main/openapi/6sense-lead-scoring-firmographics-api-openapi.yml
- filename: 6sense-people-enrichment-api-openapi.yml
  format: yaml
  label: 6sense People Enrichment API
  slug: 6sense-people-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/6sense/refs/heads/main/openapi/6sense-people-enrichment-api-openapi.yml
- filename: 6sense-people-search-api-openapi.yml
  format: yaml
  label: 6sense People Search API
  slug: 6sense-people-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/6sense/refs/heads/main/openapi/6sense-people-search-api-openapi.yml
consequence_counts:
  read: 2
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: 6Sense Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: '6sense exposes 7 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: 6sense
provider_slug: 6sense
slug: 6sense-agentic-access
source_filename: 6sense-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/6sense-company-firmographics-api-openapi.yml, openapi/6sense-company-identification-api-openapi.yml,\n  openapi/6sense-lead-scoring-api-openapi.yml, openapi/6sense-lead-scoring-firmographics-api-openapi.yml,\n  openapi/6sense-people-enrichment-api-openapi.yml, openapi/6sense-people-search-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    acting: 5\n    connected: 2\n  by_consequence:\n    write: 5\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/enrichment/company\n  method: post\n  operationId: enrichCompany\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/company/details\n  method: get\n  operationId: getCompanyDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/people/score\n  method: post\n  operationId: scoreLead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/people/full\n  method: post\n  operationId: getFullLeadData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/enrichment/people\n  method: post\n  operationId: enrichPeople\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/people/search\n  method: post\n  operationId: searchPeople\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/people/search/dictionary\n  method: get\n  operationId: getSearchDictionary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/6sense/refs/heads/main/agentic-access/6sense-agentic-access.yml
summary_line: 7 operations · 5 acting
tags:
- ABM
- Account-Based Marketing
- Intent Data
- B2B
- Predictive Analytics
- Revenue
- Sales Intelligence
- AI
- Marketing Technology
---
