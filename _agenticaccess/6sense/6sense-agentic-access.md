---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 8
api_specs:
- filename: 6sense-company-api-openapi.yml
  format: yaml
  label: 6sense Company API
  slug: 6sense-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/6sense/refs/heads/main/openapi/6sense-company-api-openapi.yml
- filename: 6sense-enrichment-api-openapi.yml
  format: yaml
  label: 6sense Enrichment API
  slug: 6sense-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/6sense/refs/heads/main/openapi/6sense-enrichment-api-openapi.yml
- filename: 6sense-people-api-openapi.yml
  format: yaml
  label: 6sense People API
  slug: 6sense-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/6sense/refs/heads/main/openapi/6sense-people-api-openapi.yml
- filename: 6sense-scoring-api-openapi.yml
  format: yaml
  label: 6sense Scoring API
  slug: 6sense-scoring-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/6sense/refs/heads/main/openapi/6sense-scoring-api-openapi.yml
consequence_counts:
  read: 8
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: 6Sense Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: '6sense exposes 16 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: 6sense
provider_slug: 6sense
slug: 6sense-agentic-access
source_filename: 6sense-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/6sense-company-api-openapi.yml, openapi/6sense-enrichment-api-openapi.yml, openapi/6sense-people-api-openapi.yml,\n  openapi/6sense-scoring-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 8\n    acting: 8\n  by_consequence:\n    read: 8\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /v3/company/details\n  method: get\n  operationId: getCompanyDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/company/products\n  method: get\n  operationId: getProductsList\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company/v1/segment/{segment_id}\n  method: get\n  operationId: getAccountsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company/v1/segments\n  method: get\n  operationId: getSegments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/company/segment/{segment_id}\n  method: get\n  operationId: getAccountsList_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/company/segments\n  method: get\n  operationId: getSegments_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/company/validate_access/segments\n  method: get\n  operationId: validateSegment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/enrichment/people\n  method: post\n  operationId: enrichPeople\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/enrichment/company\n  method: post\n  operationId: companyFirmographics\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/people/search\n\
  \  method: post\n  operationId: searchPeople\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/people/search/dictionary\n  method: get\n  operationId: getSearchDictionary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/people/enrichment\n  method: post\n  operationId: getEnrichment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/people/score\n  method: post\n  operationId: getScore\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/people/full\n  method: post\n  operationId: getScoreAndEnrichment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/people\n  method: post\n  operationId: scoreV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/scoring/people\n  method: post\n  operationId:\
  \ score\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/6sense/refs/heads/main/agentic-access/6sense-agentic-access.yml
summary_line: 16 operations · 8 acting
tags:
- Account Based Marketing
- Intent Data
- B2B
- Predictive Analytics
- Revenue
- Sales Intelligence
- Artificial Intelligence
- Marketing Technology
---
