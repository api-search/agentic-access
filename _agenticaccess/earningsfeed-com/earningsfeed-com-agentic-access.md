---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 9
api_specs:
- filename: earningsfeed-com-account-api-openapi.yml
  format: yaml
  label: Earnings Feed Account API
  slug: earningsfeed-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/earningsfeed-com/openapi/earningsfeed-com-account-api-openapi.yml
- filename: earningsfeed-com-companies-api-openapi.yml
  format: yaml
  label: Earnings Feed Companies API
  slug: earningsfeed-com-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/earningsfeed-com/openapi/earningsfeed-com-companies-api-openapi.yml
- filename: earningsfeed-com-filings-api-openapi.yml
  format: yaml
  label: Earnings Feed Filings API
  slug: earningsfeed-com-filings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/earningsfeed-com/openapi/earningsfeed-com-filings-api-openapi.yml
- filename: earningsfeed-com-insider-api-openapi.yml
  format: yaml
  label: Earnings Feed Insider API
  slug: earningsfeed-com-insider-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/earningsfeed-com/openapi/earningsfeed-com-insider-api-openapi.yml
- filename: earningsfeed-com-institutional-api-openapi.yml
  format: yaml
  label: Earnings Feed Institutional API
  slug: earningsfeed-com-institutional-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/earningsfeed-com/openapi/earningsfeed-com-institutional-api-openapi.yml
- filename: earningsfeed-com-webhooks-api-openapi.yml
  format: yaml
  label: Earnings Feed Webhooks API
  slug: earningsfeed-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/earningsfeed-com/openapi/earningsfeed-com-webhooks-api-openapi.yml
consequence_counts:
  read: 9
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Earningsfeed Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'Earnings Feed exposes 11 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Earnings Feed
provider_slug: earningsfeed-com
slug: earningsfeed-com-agentic-access
source_filename: earningsfeed-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: generated\nsource: openapi/earningsfeed-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 9\n    acting: 2\n  by_consequence:\n    read: 9\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/filings\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/filings/{accession}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/insider/transactions\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/institutional/holdings\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/companies/{cik}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/companies/search\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhooks\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n  \
  \  audit: required\n- path: /api/v1/webhooks\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhooks/{id}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/webhooks/{id}/deliveries\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/me\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/earningsfeed-com/agentic-access/earningsfeed-com-agentic-access.yml
summary_line: 11 operations · 2 acting
tags:
- Finance
- SEC
- Filings
- Data
---
