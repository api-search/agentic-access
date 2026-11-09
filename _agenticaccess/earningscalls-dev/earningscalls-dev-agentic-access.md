---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 25
api_specs:
- filename: earningscalls-dev-companies-api-openapi.yml
  format: yaml
  label: earningscalls-dev Companies API
  slug: earningscalls-dev-companies-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/earningscalls-dev/openapi/earningscalls-dev-companies-api-openapi.yml
- filename: earningscalls-dev-earnings-api-openapi.yml
  format: yaml
  label: earningscalls-dev Earnings API
  slug: earningscalls-dev-earnings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/earningscalls-dev/openapi/earningscalls-dev-earnings-api-openapi.yml
- filename: earningscalls-dev-exports-api-openapi.yml
  format: yaml
  label: earningscalls-dev Exports API
  slug: earningscalls-dev-exports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/earningscalls-dev/openapi/earningscalls-dev-exports-api-openapi.yml
- filename: earningscalls-dev-issuers-api-openapi.yml
  format: yaml
  label: earningscalls-dev Issuers API
  slug: earningscalls-dev-issuers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/earningscalls-dev/openapi/earningscalls-dev-issuers-api-openapi.yml
- filename: earningscalls-dev-metadata-api-openapi.yml
  format: yaml
  label: earningscalls-dev Metadata API
  slug: earningscalls-dev-metadata-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/earningscalls-dev/openapi/earningscalls-dev-metadata-api-openapi.yml
- filename: earningscalls-dev-search-api-openapi.yml
  format: yaml
  label: earningscalls-dev Search API
  slug: earningscalls-dev-search-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/earningscalls-dev/openapi/earningscalls-dev-search-api-openapi.yml
- filename: earningscalls-dev-speakers-api-openapi.yml
  format: yaml
  label: earningscalls-dev Speakers API
  slug: earningscalls-dev-speakers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/earningscalls-dev/openapi/earningscalls-dev-speakers-api-openapi.yml
- filename: earningscalls-dev-transcripts-api-openapi.yml
  format: yaml
  label: earningscalls-dev Transcripts API
  slug: earningscalls-dev-transcripts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/earningscalls-dev/openapi/earningscalls-dev-transcripts-api-openapi.yml
- filename: earningscalls-dev-webhooks-api-openapi.yml
  format: yaml
  label: earningscalls-dev Webhooks API
  slug: earningscalls-dev-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/earningscalls-dev/openapi/earningscalls-dev-webhooks-api-openapi.yml
consequence_counts:
  physical: 1
  read: 25
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Earningscalls Dev Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/webhooks/{id}/test
operation_count: 29
overview: 'earningscalls-dev exposes 29 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 25 read, 3 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: earningscalls-dev
provider_slug: earningscalls-dev
slug: earningscalls-dev-agentic-access
source_filename: earningscalls-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/earningscalls-dev-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 29\n  by_action_class:\n    connected: 25\n    acting: 4\n  by_consequence:\n    read: 25\n    write: 3\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/earnings/latest\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/earnings/upcoming\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/earnings/calendar\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/earnings/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/earnings/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/issuers/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/companies/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/companies/ticker/{ticker}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/companies/ticker/{ticker}/latest\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/companies/{name}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/transcripts/recent\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/transcripts/{earningsId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/transcripts/{earningsId}/summary\n  method: get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/transcripts/{earningsId}/components\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/speakers/{earningsId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/search/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/search/by_ticker\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhooks/\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhooks/\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/webhooks/{id}/test\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/webhooks/{id}\n  method: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n  \
  \    human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sectors\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/industries\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/stats\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/me\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/event-types\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/v1/exchanges\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exports/x5eg6LKCsNGIm1whxlJIiZln\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exports/x5eg6LKCsNGIm1whxlJIiZln\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/earningscalls-dev/agentic-access/earningscalls-dev-agentic-access.yml
summary_line: 29 operations · 4 acting
tags:
- Company
- Finance
- Data
- Transcripts
- Earnings Calls
---
