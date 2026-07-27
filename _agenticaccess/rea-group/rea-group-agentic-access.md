---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 27
api_specs:
- filename: rea-group-oauth-openapi.yml
  format: yaml
  label: PropTrack OAuth 2.0 Token API
  slug: proptrack-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rea-group/refs/heads/main/openapi/rea-group-oauth-openapi.yml
- filename: rea-group-address-openapi.yml
  format: yaml
  label: PropTrack Address API
  slug: proptrack-address-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rea-group/refs/heads/main/openapi/rea-group-address-openapi.yml
- filename: rea-group-properties-openapi.yml
  format: yaml
  label: PropTrack Properties API
  slug: proptrack-properties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rea-group/refs/heads/main/openapi/rea-group-properties-openapi.yml
- filename: rea-group-listings-openapi.yml
  format: yaml
  label: PropTrack Listings API
  slug: proptrack-listings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rea-group/refs/heads/main/openapi/rea-group-listings-openapi.yml
- filename: rea-group-transactions-openapi.yml
  format: yaml
  label: PropTrack Transactions API
  slug: proptrack-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rea-group/refs/heads/main/openapi/rea-group-transactions-openapi.yml
- filename: rea-group-market-openapi.yml
  format: yaml
  label: PropTrack Market API
  slug: proptrack-market-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rea-group/refs/heads/main/openapi/rea-group-market-openapi.yml
- filename: rea-group-reports-openapi.yml
  format: yaml
  label: PropTrack Reports API
  slug: proptrack-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rea-group/refs/heads/main/openapi/rea-group-reports-openapi.yml
- filename: rea-group-disclaimers-openapi.yml
  format: yaml
  label: PropTrack Disclaimers API
  slug: proptrack-disclaimers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rea-group/refs/heads/main/openapi/rea-group-disclaimers-openapi.yml
- filename: rea-group-coming-soon-openapi.yml
  format: yaml
  label: PropTrack Upcoming APIs (Schools)
  slug: proptrack-upcoming-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/rea-group/refs/heads/main/openapi/rea-group-coming-soon-openapi.yml
consequence_counts:
  read: 27
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Rea Group Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 32
overview: 'REA Group exposes 32 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 27 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: REA Group
provider_slug: rea-group
slug: rea-group-agentic-access
source_filename: rea-group-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-27'\nmethod: generated\nsource: openapi/rea-group-address-openapi.yml, openapi/rea-group-coming-soon-openapi.yml, openapi/rea-group-disclaimers-openapi.yml,\n  openapi/rea-group-listings-openapi.yml, openapi/rea-group-market-openapi.yml, openapi/rea-group-oauth-openapi.yml,\n  openapi/rea-group-properties-openapi.yml, openapi/rea-group-reports-openapi.yml, openapi/rea-group-transactions-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 32\n  by_action_class:\n    connected: 27\n    acting: 5\n  by_consequence:\n    read: 27\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v2/address/match\n  method: get\n  operationId: address.match\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/address/suggest\n  method: get\n  operationId: address.suggest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/properties/{propertyId}/nearby-education-facilities\n  method: get\n  operationId: get-api-v2-properties-propertyId-nearby-education-facilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/disclaimers\n  method: get\n  operationId: get-api-v1-disclaimers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/listings/{listingId}\n  method: get\n  operationId: listings\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/listings/search/point-and-radius\n  method: get\n  operationId: listings-point-and-radius-search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/listings/search/suburb-and-postcode\n  method: get\n  operationId: get-api-v2-listings-search-suburb-and-postcode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/market/auctions\n  method: get\n  operationId: get-api-v2-market-auctions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/market/rent/historic/{metric}\n  method: get\n  operationId: market.rent-history\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/market/sale/historic/{metric}\n  method: get\n  operationId: market.sale-history\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/market/supply-and-demand/{metric}\n  method: get\n  operationId: market.supply-and-demand\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/market/demographics\n  method: get\n  operationId: /api/v2/market/demographics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth2/token\n  method: post\n  operationId: auth-token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/properties/{propertyId}/summary\n  method: get\n  operationId: get-v2-summary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/properties/{propertyId}/attributes\n  method: get\n  operationId: properties-attributes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/properties/{propertyId}/listings\n  method: get\n  operationId: listings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/properties/{propertyId}/planning\n  method: get\n  operationId: get-api-v2-properties-planning\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/properties/{propertyId}/tenureType\n  method: get\n  operationId: get-api-v2-properties-tenure\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/properties/{propertyId}/transactions\n  method: get\n  operationId: transactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/properties/valuations/sale\n  method: post\n  operationId: v1-properties-valuation-sale\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/v1/properties/{propertyId}/valuations/sale?requestType=enquiry or requestType=origination\n  method: get\n  operationId: avm-propertyId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/properties/{propertyId}/valuations/rent?requestType=enquiry or requestType=origination\n  method: get\n  operationId: avm-propertyId-enquiry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/properties/valuations/sale ~ requestType=plus\n  method: post\n  operationId: v1-properties-valuation-sale-plus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /api/v1/properties/{propertyId}/valuations/sale?requestType=plus\n  method: get\n  operationId: avm-propertyId-plus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/properties/valuations/sale ~ Pro\n  method: post\n  operationId: v1-properties-valuation-sale-pro\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/properties/{propertyId}/valuations/sale?requestType=pro\n  method: get\n  operationId: avm-propertyId-pro\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/properties/summaries/search\n\
  \  method: get\n  operationId: get-api-v2-properties-summaries-search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/properties/geopoints/search\n  method: get\n  operationId: get-api-v2-properties-geopoints-pins\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/reports/valuations/{valuationId}/pdf\n  method: get\n  operationId: reports-valuations-pdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/reports/property\n  method: post\n  operationId: reports-property-report\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/transactions/search/point-and-radius\n  method: get\n  operationId: get-transactions-propertyId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/transactions/search/suburb-and-postcode\n  method: get\n  operationId: get-transactions-propertyId-suburb\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/rea-group/refs/heads/main/agentic-access/rea-group-agentic-access.yml
summary_line: 32 operations · 5 acting
tags:
- Real Estate
- Property Data
- Valuations
- AVM
- Market Insights
- Listings
- Transactions
- Address Matching
- REAXML
- Partner Portal
- PropTech
- Australia
---
