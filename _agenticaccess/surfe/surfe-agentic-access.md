---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 3
api_specs:
- filename: surfe-openapi.yml
  format: yaml
  label: Surfe People Search API
  slug: surfe-people-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surfe/refs/heads/main/openapi/surfe-openapi.yml
- filename: surfe-openapi.yml
  format: yaml
  label: Surfe People Enrichment API
  slug: surfe-people-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surfe/refs/heads/main/openapi/surfe-openapi.yml
- filename: surfe-openapi.yml
  format: yaml
  label: Surfe Company Search API
  slug: surfe-company-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surfe/refs/heads/main/openapi/surfe-openapi.yml
- filename: surfe-openapi.yml
  format: yaml
  label: Surfe Company Enrichment API
  slug: surfe-company-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surfe/refs/heads/main/openapi/surfe-openapi.yml
- filename: surfe-openapi.yml
  format: yaml
  label: Surfe Recommendations API
  slug: surfe-recommendations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surfe/refs/heads/main/openapi/surfe-openapi.yml
- filename: surfe-openapi.yml
  format: yaml
  label: Surfe Credits API
  slug: surfe-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/surfe/refs/heads/main/openapi/surfe-openapi.yml
consequence_counts:
  read: 3
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Surfe Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'Surfe exposes 10 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Surfe
provider_slug: surfe
slug: surfe-agentic-access
source_filename: surfe-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/surfe-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 7\n    connected: 3\n  by_consequence:\n    write: 7\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /people/search\n  method: post\n  operationId: searchPeople\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /people/enrich\n  method: post\n  operationId: startPeopleEnrichment\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /people/enrich/{id}\n  method: get\n  operationId: getPeopleEnrichment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /people/find-by-email\n  method: post\n  operationId: findPeopleByEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/search\n  method: post\n  operationId: searchCompanies\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/enrich\n  method: post\n  operationId: startCompanyEnrichment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/enrich/{id}\n  method: get\n  operationId: getCompanyEnrichment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /recommendations/icp\n  method: post\n  operationId: upsertICP\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /recommendations/fetch\n  method: post\n  operationId: fetchRecommendations\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /credits\n  method: get\n  operationId: getCredits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/surfe/refs/heads/main/agentic-access/surfe-agentic-access.yml
summary_line: 10 operations · 7 acting
tags:
- B2B Data
- Contact Data
- Sales Intelligence
- Enrichment
- Lead Generation
- CRM
- Prospecting
---
