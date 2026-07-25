---
acting_count: 0
action_class_counts:
  connected: 11
api_specs:
- filename: chicago-transit-authority-arrivals-api-openapi.yml
  format: yaml
  label: Chicago Transit Authority Arrivals API
  slug: chicago-transit-authority-arrivals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chicago-transit-authority/refs/heads/main/openapi/chicago-transit-authority-arrivals-api-openapi.yml
- filename: chicago-transit-authority-bulletins-api-openapi.yml
  format: yaml
  label: Chicago Transit Authority Bulletins API
  slug: chicago-transit-authority-bulletins-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chicago-transit-authority/refs/heads/main/openapi/chicago-transit-authority-bulletins-api-openapi.yml
- filename: chicago-transit-authority-follow-api-openapi.yml
  format: yaml
  label: Chicago Transit Authority Follow API
  slug: chicago-transit-authority-follow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chicago-transit-authority/refs/heads/main/openapi/chicago-transit-authority-follow-api-openapi.yml
- filename: chicago-transit-authority-locations-api-openapi.yml
  format: yaml
  label: Chicago Transit Authority Locations API
  slug: chicago-transit-authority-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chicago-transit-authority/refs/heads/main/openapi/chicago-transit-authority-locations-api-openapi.yml
- filename: chicago-transit-authority-predictions-api-openapi.yml
  format: yaml
  label: Chicago Transit Authority Predictions API
  slug: chicago-transit-authority-predictions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chicago-transit-authority/refs/heads/main/openapi/chicago-transit-authority-predictions-api-openapi.yml
- filename: chicago-transit-authority-routes-api-openapi.yml
  format: yaml
  label: Chicago Transit Authority Routes API
  slug: chicago-transit-authority-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chicago-transit-authority/refs/heads/main/openapi/chicago-transit-authority-routes-api-openapi.yml
- filename: chicago-transit-authority-stops-api-openapi.yml
  format: yaml
  label: Chicago Transit Authority Stops API
  slug: chicago-transit-authority-stops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chicago-transit-authority/refs/heads/main/openapi/chicago-transit-authority-stops-api-openapi.yml
- filename: chicago-transit-authority-system-api-openapi.yml
  format: yaml
  label: Chicago Transit Authority System API
  slug: chicago-transit-authority-system-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chicago-transit-authority/refs/heads/main/openapi/chicago-transit-authority-system-api-openapi.yml
- filename: chicago-transit-authority-vehicles-api-openapi.yml
  format: yaml
  label: Chicago Transit Authority Vehicles API
  slug: chicago-transit-authority-vehicles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/chicago-transit-authority/refs/heads/main/openapi/chicago-transit-authority-vehicles-api-openapi.yml
consequence_counts:
  read: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Chicago Transit Authority Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'Chicago Transit Authority exposes 11 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Chicago Transit Authority
provider_slug: chicago-transit-authority
slug: chicago-transit-authority-agentic-access
source_filename: chicago-transit-authority-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/cta-bus-tracker-openapi.yml, openapi/cta-train-tracker-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 11\n  by_consequence:\n    read: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /gettime\n  method: get\n  operationId: getTime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getroutes\n  method: get\n  operationId: getRoutes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getdirections\n  method: get\n  operationId:\
  \ getDirections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getstops\n  method: get\n  operationId: getStops\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getpatterns\n  method: get\n  operationId: getPatterns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getvehicles\n  method: get\n  operationId: getVehicles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getpredictions\n  method: get\n  operationId: getPredictions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /getservicebulletins\n  method: get\n  operationId: getServiceBulletins\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ttarrivals.aspx\n  method: get\n  operationId: getArrivals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ttfollow.aspx\n  method: get\n  operationId: followTrain\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ttpositions.aspx\n  method: get\n  operationId: getPositions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/chicago-transit-authority/refs/heads/main/agentic-access/chicago-transit-authority-agentic-access.yml
summary_line: 11 operations
tags:
- Bus
- Bus Tracker
- Chicago
- CTA
- Customer Alerts
- GTFS
- L Train
- Open Data
- Public Transit
- Real-Time
- Train
- Train Tracker
- Transit
- Transportation
---
