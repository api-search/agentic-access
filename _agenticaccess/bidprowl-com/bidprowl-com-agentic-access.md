---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 10
api_specs:
- filename: bidprowl-com-comps-api-openapi.yml
  format: yaml
  label: BidProwl Comps API
  slug: bidprowl-com-comps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bidprowl-com/openapi/bidprowl-com-comps-api-openapi.yml
- filename: bidprowl-com-export-api-openapi.yml
  format: yaml
  label: BidProwl Export API
  slug: bidprowl-com-export-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bidprowl-com/openapi/bidprowl-com-export-api-openapi.yml
- filename: bidprowl-com-flip-score-api-openapi.yml
  format: yaml
  label: BidProwl Flip Score API
  slug: bidprowl-com-flip-score-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bidprowl-com/openapi/bidprowl-com-flip-score-api-openapi.yml
- filename: bidprowl-com-listings-api-openapi.yml
  format: yaml
  label: BidProwl Listings API
  slug: bidprowl-com-listings-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bidprowl-com/openapi/bidprowl-com-listings-api-openapi.yml
- filename: bidprowl-com-sold-api-openapi.yml
  format: yaml
  label: BidProwl Sold API
  slug: bidprowl-com-sold-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bidprowl-com/openapi/bidprowl-com-sold-api-openapi.yml
- filename: bidprowl-com-sources-api-openapi.yml
  format: yaml
  label: BidProwl Sources API
  slug: bidprowl-com-sources-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bidprowl-com/openapi/bidprowl-com-sources-api-openapi.yml
- filename: bidprowl-com-usage-api-openapi.yml
  format: yaml
  label: BidProwl Usage API
  slug: bidprowl-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bidprowl-com/openapi/bidprowl-com-usage-api-openapi.yml
- filename: bidprowl-com-webhooks-api-openapi.yml
  format: yaml
  label: BidProwl Webhooks API
  slug: bidprowl-com-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/bidprowl-com/openapi/bidprowl-com-webhooks-api-openapi.yml
consequence_counts:
  read: 10
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bidprowl Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'BidProwl exposes 12 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BidProwl
provider_slug: bidprowl-com
slug: bidprowl-com-agentic-access
source_filename: bidprowl-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/bidprowl-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 10\n    acting: 2\n  by_consequence:\n    read: 10\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/listings\n  method: get\n  operationId: searchListings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/listings/{id}\n  method: get\n  operationId: getListing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sources\n  method:\
  \ get\n  operationId: listSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/comps\n  method: get\n  operationId: getSoldComps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/comps/batch\n  method: post\n  operationId: getSoldCompsBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sold\n  method: get\n  operationId: listSoldLots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/webhooks/{id}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/flip-score/{id}\n  method:\
  \ get\n  operationId: getFlipScore\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/export\n  method: get\n  operationId: exportListingsCsv\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/bidprowl-com/agentic-access/bidprowl-com-agentic-access.yml
summary_line: 12 operations · 2 acting
tags:
- Government
- Auctions
- Marketplace
- Data
- Search
---
