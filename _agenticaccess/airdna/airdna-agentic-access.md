---
acting_count: 22
action_class_counts:
  acting: 22
  connected: 4
api_specs:
- filename: airdna-openapi.yml
  format: yaml
  label: AirDNA Market Search
  slug: market-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airdna/refs/heads/main/openapi/airdna-openapi.yml
- filename: airdna-openapi.yml
  format: yaml
  label: AirDNA Market Stats
  slug: market-stats
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airdna/refs/heads/main/openapi/airdna-openapi.yml
- filename: airdna-openapi.yml
  format: yaml
  label: AirDNA Property/Listing Data
  slug: property-listing-data
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airdna/refs/heads/main/openapi/airdna-openapi.yml
- filename: airdna-openapi.yml
  format: yaml
  label: AirDNA Rentalizer Estimates
  slug: rentalizer-estimates
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airdna/refs/heads/main/openapi/airdna-openapi.yml
- filename: airdna-openapi.yml
  format: yaml
  label: AirDNA Comps
  slug: comps
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/airdna/refs/heads/main/openapi/airdna-openapi.yml
consequence_counts:
  read: 4
  write: 22
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Airdna Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 26
overview: 'AirDNA exposes 26 API operations that an AI agent could call, of which 22 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 22 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AirDNA
provider_slug: airdna
slug: airdna-agentic-access
source_filename: airdna-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/airdna-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 26\n  by_action_class:\n    acting: 22\n    connected: 4\n  by_consequence:\n    write: 22\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /market/search\n  method: post\n  operationId: searchMarkets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /market/{marketId}\n  method: get\n  operationId: getMarket\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /country/{countryCode}/markets\n  method: post\n  operationId: exploreCountryMarkets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /market/{marketId}/metrics/occupancy\n  method: post\n  operationId: getMarketOccupancy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /market/{marketId}/metrics/revenue\n  method: post\n  operationId: getMarketRevenue\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /market/{marketId}/metrics/adr\n  method: post\n  operationId: getMarketAdr\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /market/{marketId}/metrics/revpar\n  method: post\n  operationId: getMarketRevpar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /market/{marketId}/metrics/booking-lead-time\n  method: post\n  operationId:\
  \ getMarketBookingLeadTime\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /market/{marketId}/metrics/length-of-stay\n  method: post\n  operationId: getMarketLengthOfStay\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /market/{marketId}/metrics/active-listings\n  method: post\n  operationId: getMarketActiveListings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n   \
  \   triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /market/{marketId}/pricing/future\n  method: post\n  operationId: getMarketFuturePricing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /submarket/{submarketId}\n  method: get\n  operationId: getSubmarket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /market/{marketId}/submarkets\n  method: post\n  operationId: exploreMarketSubmarkets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /listing/search\n  method: post\n  operationId: searchListings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /market/{marketId}/listings\n  method: post\n  operationId: exploreMarketListings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listings/radius\n  method: post\n  operationId: exploreListingsRadius\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listing/{listingId}\n  method: get\n  operationId: getListing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /listings/details\n  method: post\n  operationId: getListingsDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listing/{listingId}/metrics/historical\n  method: post\n  operationId: getListingHistoricalMetrics\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n \
  \     triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listing/{listingId}/comps\n  method: post\n  operationId: getListingComps\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listing/{listingId}/pricing/future\n  method: post\n  operationId: getListingFuturePricing\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rentalizer/individual\n  method: post\n  operationId: rentalizerIndividual\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rentalizer/bulk\n  method: post\n  operationId: rentalizerBulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rentalizer-lead-gen/summary\n  method: post\n  operationId: rentalizerLeadGenSummary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /smart-rates/{listingId}\n  method: get\n  operationId: getSmartRatesBase\n  x-agentic-access:\n  \
  \  action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /smart-rates/{listingId}\n  method: post\n  operationId: getSmartRates\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/airdna/refs/heads/main/agentic-access/airdna-agentic-access.yml
summary_line: 26 operations · 22 acting
tags:
- Short-Term Rental
- Vacation Rental
- Market Data
- Real Estate
- Analytics
---
