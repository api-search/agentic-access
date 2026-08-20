---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 21
api_specs:
- filename: zillapi-account-api-openapi.yml
  format: yaml
  label: Zillapi Account API
  slug: zillapi-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zillapi/refs/heads/main/openapi/zillapi-account-api-openapi.yml
- filename: zillapi-buildings-api-openapi.yml
  format: yaml
  label: Zillapi Buildings API
  slug: zillapi-buildings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zillapi/refs/heads/main/openapi/zillapi-buildings-api-openapi.yml
- filename: zillapi-jobs-api-openapi.yml
  format: yaml
  label: Zillapi Jobs API
  slug: zillapi-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zillapi/refs/heads/main/openapi/zillapi-jobs-api-openapi.yml
- filename: zillapi-listings-api-openapi.yml
  format: yaml
  label: Zillapi Listings API
  slug: zillapi-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zillapi/refs/heads/main/openapi/zillapi-listings-api-openapi.yml
- filename: zillapi-properties-api-openapi.yml
  format: yaml
  label: Zillapi Properties API
  slug: zillapi-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zillapi/refs/heads/main/openapi/zillapi-properties-api-openapi.yml
- filename: zillapi-search-api-openapi.yml
  format: yaml
  label: Zillapi Search API
  slug: zillapi-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zillapi/refs/heads/main/openapi/zillapi-search-api-openapi.yml
- filename: zillapi-webhooks-api-openapi.yml
  format: yaml
  label: Zillapi Webhooks API
  slug: zillapi-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/zillapi/refs/heads/main/openapi/zillapi-webhooks-api-openapi.yml
consequence_counts:
  read: 21
  safety-critical: 1
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Zillapi Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/webhooks/{id}
operation_count: 29
overview: 'Zillapi exposes 29 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read, 7 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Zillapi
provider_slug: zillapi
slug: zillapi-agentic-access
source_filename: zillapi-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-09'\nmethod: generated\nsource: openapi/zillapi-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 29\n  by_action_class:\n    connected: 21\n    acting: 8\n  by_consequence:\n    read: 21\n    write: 7\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /v1/properties/by-url\n  method: get\n  operationId: getPropertyByUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/properties/by-address\n  method: get\n  operationId: getPropertyByAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/properties/{zpid}\n  method: get\n  operationId: getPropertyByZpid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/properties/{zpid}/photos\n  method: get\n  operationId: getPropertyPhotos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/properties/{zpid}/price-history\n  method: get\n  operationId: getPropertyPriceHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/properties/{zpid}/tax-history\n  method: get\n  operationId: getPropertyTaxHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/properties/{zpid}/schools\n\
  \  method: get\n  operationId: getPropertySchools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/properties/{zpid}/nearby\n  method: get\n  operationId: getPropertyNearby\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/properties/{zpid}/agent\n  method: get\n  operationId: getPropertyAgent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/properties/{zpid}/zestimate\n  method: get\n  operationId: getPropertyZestimate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/properties/{zpid}/open-houses\n  method: get\n  operationId: getPropertyOpenHouses\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/properties/{zpid}/facts\n  method: get\n  operationId: getPropertyFacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/properties/batch\n  method: post\n  operationId: createBatchPropertyJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/buildings/by-url\n  method: get\n  operationId: getBuildingByUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/listings/for-sale\n  method: post\n  operationId:\
  \ listingsForSale\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/listings/for-rent\n  method: post\n  operationId: listingsForRent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/listings/sold\n  method: post\n  operationId: listingsSold\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/listings\n  method: get\n  operationId: listingsBbox\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/search\n  method: post\n  operationId: search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/search/with-details\n  method: post\n  operationId: searchWithDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/jobs\n  method: get\n  operationId: listJobs\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{id}\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/jobs/{id}/results\n  method: get\n  operationId: getJobResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/webhooks/{id}\n  method: delete\n  operationId: revokeWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/webhooks/{id}/deliveries\n  method: get\n  operationId: listWebhookDeliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/zillapi/refs/heads/main/agentic-access/zillapi-agentic-access.yml
summary_line: 29 operations · 8 acting · 1 human-in-the-loop
tags:
- Real-Estate
- PropTech
- Property Data
- Zillow
- Zestimate
- Valuation
- AVM
- Listings
- MCP
- AI Agent
- REST API
---
