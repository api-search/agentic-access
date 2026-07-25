---
acting_count: 0
action_class_counts:
  connected: 6
api_specs:
- filename: amadeus-traveler-media-category-rated-areas-api-openapi.yml
  format: yaml
  label: Amadeus Traveler Media category-rated-areas API
  slug: amadeus-traveler-media-category-rated-areas-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/openapi/amadeus-traveler-media-category-rated-areas-api-openapi.yml
- filename: amadeus-traveler-media-hotel-ratings-api-openapi.yml
  format: yaml
  label: Amadeus Traveler Media Hotel Ratings API
  slug: amadeus-traveler-media-hotel-ratings-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/openapi/amadeus-traveler-media-hotel-ratings-api-openapi.yml
- filename: amadeus-traveler-media-recommended-locations-api-openapi.yml
  format: yaml
  label: Amadeus Traveler Media recommended-locations API
  slug: amadeus-traveler-media-recommended-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/openapi/amadeus-traveler-media-recommended-locations-api-openapi.yml
- filename: amadeus-traveler-media-retrieve-api-openapi.yml
  format: yaml
  label: Amadeus Traveler Media Retrieve API
  slug: amadeus-traveler-media-retrieve-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/openapi/amadeus-traveler-media-retrieve-api-openapi.yml
- filename: amadeus-traveler-media-search-api-openapi.yml
  format: yaml
  label: Amadeus Traveler Media Search API
  slug: amadeus-traveler-media-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/openapi/amadeus-traveler-media-search-api-openapi.yml
consequence_counts:
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Amadeus Traveler Media Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Amadeus Traveler Media exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Amadeus Traveler Media
provider_slug: amadeus-traveler-media
slug: amadeus-traveler-media-agentic-access
source_filename: amadeus-traveler-media-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/amadeus-traveler-media-hotel-ratings-openapi.yaml, openapi/amadeus-traveler-media-location-score-openapi.yaml,\n  openapi/amadeus-traveler-media-points-of-interest-openapi.yaml, openapi/amadeus-traveler-media-travel-recommendations-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 6\n  by_consequence:\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /e-reputation/hotel-sentiments\n  method: get\n  operationId: getSentimentsByHotelIds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /location/analytics/category-rated-areas\n\
  \  method: get\n  operationId: get-category-rated-areas\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reference-data/locations/pois\n  method: get\n  operationId: getPointsOfInterest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reference-data/locations/pois/{poisId}\n  method: get\n  operationId: getPointOfInterest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reference-data/locations/pois/by-square\n  method: get\n  operationId: getPointsOfInterestBySquare\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reference-data/recommended-locations\n  method: get\n\
  \  operationId: getRecommendedLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/amadeus-traveler-media/refs/heads/main/agentic-access/amadeus-traveler-media-agentic-access.yml
summary_line: 6 operations
tags:
- Content
- Destination
- Media
- Photos
- Points of Interest
- Tourism
- Travel
---
