---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 9
api_specs:
- filename: rocketreach-people-lookup-api-openapi.yml
  format: yaml
  label: RocketReach People Lookup API
  slug: rocketreach-people-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocketreach/refs/heads/main/openapi/rocketreach-people-lookup-api-openapi.yml
- filename: rocketreach-people-search-api-openapi.yml
  format: yaml
  label: RocketReach People Search API
  slug: rocketreach-people-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocketreach/refs/heads/main/openapi/rocketreach-people-search-api-openapi.yml
- filename: rocketreach-company-lookup-api-openapi.yml
  format: yaml
  label: RocketReach Company Lookup API
  slug: rocketreach-company-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocketreach/refs/heads/main/openapi/rocketreach-company-lookup-api-openapi.yml
- filename: rocketreach-company-search-api-openapi.yml
  format: yaml
  label: RocketReach Company Search API
  slug: rocketreach-company-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocketreach/refs/heads/main/openapi/rocketreach-company-search-api-openapi.yml
- filename: rocketreach-account-api-openapi.yml
  format: yaml
  label: RocketReach Account API
  slug: rocketreach-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rocketreach/refs/heads/main/openapi/rocketreach-account-api-openapi.yml
consequence_counts:
  read: 9
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Rocketreach Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 16
overview: 'RocketReach exposes 16 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 7 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: RocketReach
provider_slug: rocketreach
slug: rocketreach-agentic-access
source_filename: rocketreach-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/rocketreach-account-api-openapi.yml, openapi/rocketreach-company-lookup-api-openapi.yml,\n  openapi/rocketreach-company-search-api-openapi.yml, openapi/rocketreach-people-lookup-api-openapi.yml,\n  openapi/rocketreach-people-search-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 16\n  by_action_class:\n    connected: 9\n    acting: 7\n  by_consequence:\n    read: 9\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /account/\n  method: get\n  operationId: get_account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/key/\n  method: post\n\
  \  operationId: create_new_api_key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /universal/account/\n  method: get\n  operationId: get_universal_account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /company/lookup/\n  method: get\n  operationId: create_company_lookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /universal/company/lookup\n  method: get\n  operationId: create_universal_company_lookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /searchCompany\n  method: post\n  operationId: create_company_search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /universal/company/search\n  method: post\n  operationId: create_universal_company_search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /person/lookup\n  method: get\n  operationId: create_person_lookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /person/checkStatus\n  method:\
  \ get\n  operationId: check_person_lookup_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bulkLookup\n  method: post\n  operationId: create_person_bulk_lookup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /profile-company/lookup\n  method: get\n  operationId: create_person_and_company_lookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /universal/person/lookup\n  method: get\n  operationId: create_universal_person_lookup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /universal/person/bulk_lookup\n  method: post\n  operationId: create_universal_person_bulk_lookup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /universal/person/check_status\n  method: get\n  operationId: check_universal_person_lookup_status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /person/search\n  method: post\n  operationId: create_person_search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /universal/person/search\n  method: post\n  operationId: create_universal_person_search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rocketreach/refs/heads/main/agentic-access/rocketreach-agentic-access.yml
summary_line: 16 operations · 7 acting
tags:
- B2B
- Contact Data
- Email Lookup
- Phone Lookup
- Sales Intelligence
- Lead Generation
- People Search
- Company Search
- Data Enrichment
- Prospecting
- Recruiting
- Webhooks
---
