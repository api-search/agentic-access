---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 18
api_specs:
- filename: roote-capabilities-api-openapi.yml
  format: yaml
  label: ROOTE Capabilities API
  slug: roote-capabilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roote/refs/heads/main/openapi/roote-capabilities-api-openapi.yml
- filename: roote-changelog-json-api-openapi.yml
  format: yaml
  label: ROOTE Changelog.json API
  slug: roote-changelog-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roote/refs/heads/main/openapi/roote-changelog-json-api-openapi.yml
- filename: roote-charging-api-openapi.yml
  format: yaml
  label: ROOTE Charging API
  slug: roote-charging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roote/refs/heads/main/openapi/roote-charging-api-openapi.yml
- filename: roote-geocode-api-openapi.yml
  format: yaml
  label: ROOTE Geocode API
  slug: roote-geocode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roote/refs/heads/main/openapi/roote-geocode-api-openapi.yml
- filename: roote-health-api-openapi.yml
  format: yaml
  label: ROOTE Health API
  slug: roote-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roote/refs/heads/main/openapi/roote-health-api-openapi.yml
- filename: roote-mobility-api-openapi.yml
  format: yaml
  label: ROOTE Mobility API
  slug: roote-mobility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roote/refs/heads/main/openapi/roote-mobility-api-openapi.yml
- filename: roote-nearby-api-openapi.yml
  format: yaml
  label: ROOTE Nearby API
  slug: roote-nearby-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roote/refs/heads/main/openapi/roote-nearby-api-openapi.yml
- filename: roote-openapi-json-api-openapi.yml
  format: yaml
  label: ROOTE Openapi.json API
  slug: roote-openapi-json-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roote/refs/heads/main/openapi/roote-openapi-json-api-openapi.yml
- filename: roote-parking-api-openapi.yml
  format: yaml
  label: ROOTE Parking API
  slug: roote-parking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roote/refs/heads/main/openapi/roote-parking-api-openapi.yml
- filename: roote-place-search-api-openapi.yml
  format: yaml
  label: ROOTE Place Search API
  slug: roote-place-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roote/refs/heads/main/openapi/roote-place-search-api-openapi.yml
- filename: roote-reverse-geocode-api-openapi.yml
  format: yaml
  label: ROOTE Reverse Geocode API
  slug: roote-reverse-geocode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roote/refs/heads/main/openapi/roote-reverse-geocode-api-openapi.yml
- filename: roote-ride-hailing-api-openapi.yml
  format: yaml
  label: ROOTE Ride Hailing API
  slug: roote-ride-hailing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roote/refs/heads/main/openapi/roote-ride-hailing-api-openapi.yml
- filename: roote-services-api-openapi.yml
  format: yaml
  label: ROOTE Services API
  slug: roote-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roote/refs/heads/main/openapi/roote-services-api-openapi.yml
- filename: roote-transit-api-openapi.yml
  format: yaml
  label: ROOTE Transit API
  slug: roote-transit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roote/refs/heads/main/openapi/roote-transit-api-openapi.yml
- filename: roote-usage-api-openapi.yml
  format: yaml
  label: ROOTE Usage API
  slug: roote-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/roote/refs/heads/main/openapi/roote-usage-api-openapi.yml
consequence_counts:
  physical: 1
  read: 18
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Roote Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/transit/journey
operation_count: 20
overview: 'ROOTE exposes 20 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read, 1 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ROOTE
provider_slug: roote
slug: roote-agentic-access
source_filename: roote-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-05'\nmethod: generated\nsource: openapi/roote-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    connected: 18\n    acting: 2\n  by_consequence:\n    read: 18\n    physical: 1\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /health\n  method: get\n  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /changelog.json\n  method: get\n  operationId: getChangelog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/nearby\n  method: get\n  operationId:\
  \ getGlobalNearby\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi.json\n  method: get\n  operationId: openApi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /usage/cities\n  method: get\n  operationId: publicCityUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/geocode\n  method: get\n  operationId: geocodeAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/place-search\n  method: get\n  operationId: searchPlaces\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/reverse-geocode\n  method: get\n  operationId: reverseGeocode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/services/nearby\n  method: get\n  operationId: getNearbyServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/parking/nearby\n  method: get\n  operationId: getNearbyParking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/charging/nearby\n  method: get\n  operationId: getNearbyEvCharging\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transit/nearby\n  method: get\n  operationId: getNearbyTransport\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transit/lines/{id}/patterns\n  method: get\n  operationId: getTransportLinePatterns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transit/stations/{id}\n  method: get\n  operationId: getTransportStation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transit/stations/{id}/departures\n  method: get\n  operationId: getTransportDepartures\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transit/journey\n  method: get\n  operationId: getTransportJourney\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transit/journey\n  method: post\n  operationId: createTransportJourney\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ride-hailing/estimates\n  method: get\n  operationId: getRideHailingEstimates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/capabilities\n  method: post\n  operationId: runCapability\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/mobility/nearby\n  method: get\n  operationId: getNearbyMobility\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/roote/refs/heads/main/agentic-access/roote-agentic-access.yml
summary_line: 20 operations · 2 acting
tags:
- Mobility
- French
- Artificial Intelligence
- Transportation
---
