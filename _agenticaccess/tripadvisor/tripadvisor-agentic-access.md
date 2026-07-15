---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 7
api_specs:
- filename: tripadvisor-content-api-openapi.yml
  format: yaml
  label: Tripadvisor Content API
  slug: content-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tripadvisor/refs/heads/main/openapi/tripadvisor-content-api-openapi.yml
- filename: tripadvisor-hotel-availability-check-api-openapi.yml
  format: yaml
  label: Tripadvisor Hotel Availability Check API
  slug: hotel-availability-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tripadvisor/refs/heads/main/openapi/tripadvisor-hotel-availability-check-api-openapi.yml
- filename: tripadvisor-hotel-availability-check-api-openapi.yml
  format: yaml
  label: Tripadvisor Hotel Inventory API
  slug: hotel-inventory-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tripadvisor/refs/heads/main/openapi/tripadvisor-hotel-availability-check-api-openapi.yml
consequence_counts:
  read: 7
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tripadvisor Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Tripadvisor exposes 8 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Tripadvisor
provider_slug: tripadvisor
slug: tripadvisor-agentic-access
source_filename: tripadvisor-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/tripadvisor-content-api-openapi.yml, openapi/tripadvisor-hotel-availability-check-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 7\n    acting: 1\n  by_consequence:\n    read: 7\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /location/search\n  method: get\n  operationId: searchForLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /location/nearby_search\n  method: get\n  operationId: searchForNearbyLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /location/{locationId}/details\n  method: get\n  operationId: getLocationDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /location/{locationId}/photos\n  method: get\n  operationId: getLocationPhotos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /location/{locationId}/reviews\n  method: get\n  operationId: getLocationReviews\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /config\n  method: get\n  operationId: getConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hotel_inventory\n\
  \  method: get\n  operationId: getHotelInventory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /availability\n  method: post\n  operationId: checkAvailability\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tripadvisor/refs/heads/main/agentic-access/tripadvisor-agentic-access.yml
summary_line: 8 operations · 1 acting
tags:
- Attractions
- Hotels
- Hospitality
- Restaurants
- Reviews
- Travel
---
