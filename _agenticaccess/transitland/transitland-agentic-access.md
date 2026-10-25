---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 28
api_specs:
- filename: transitland-agencies-api-openapi.yml
  format: yaml
  label: TransitLand Agencies API
  slug: transitland-agencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transitland/refs/heads/main/openapi/transitland-agencies-api-openapi.yml
- filename: transitland-feed-versions-api-openapi.yml
  format: yaml
  label: TransitLand Feed Versions API
  slug: transitland-feed-versions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transitland/refs/heads/main/openapi/transitland-feed-versions-api-openapi.yml
- filename: transitland-feeds-api-openapi.yml
  format: yaml
  label: TransitLand Feeds API
  slug: transitland-feeds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transitland/refs/heads/main/openapi/transitland-feeds-api-openapi.yml
- filename: transitland-onestop-id-api-openapi.yml
  format: yaml
  label: TransitLand Onestop Id API
  slug: transitland-onestop-id-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transitland/refs/heads/main/openapi/transitland-onestop-id-api-openapi.yml
- filename: transitland-operators-api-openapi.yml
  format: yaml
  label: TransitLand Operators API
  slug: transitland-operators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transitland/refs/heads/main/openapi/transitland-operators-api-openapi.yml
- filename: transitland-routes-api-openapi.yml
  format: yaml
  label: TransitLand Routes API
  slug: transitland-routes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transitland/refs/heads/main/openapi/transitland-routes-api-openapi.yml
- filename: transitland-stops-api-openapi.yml
  format: yaml
  label: TransitLand Stops API
  slug: transitland-stops-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transitland/refs/heads/main/openapi/transitland-stops-api-openapi.yml
- filename: transitland-street-routing-api-openapi.yml
  format: yaml
  label: TransitLand Street routing API
  slug: transitland-street-routing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transitland/refs/heads/main/openapi/transitland-street-routing-api-openapi.yml
- filename: transitland-transit-routing-api-openapi.yml
  format: yaml
  label: TransitLand Transit routing API
  slug: transitland-transit-routing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/transitland/refs/heads/main/openapi/transitland-transit-routing-api-openapi.yml
consequence_counts:
  read: 28
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Transitland Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 37
overview: 'TransitLand exposes 37 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 28 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: TransitLand
provider_slug: transitland
slug: transitland-agentic-access
source_filename: transitland-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-19'\nmethod: generated\nsource: openapi/transitland-rest-openapi.yml, openapi/transitland-routing-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 37\n  by_action_class:\n    connected: 28\n    acting: 9\n  by_consequence:\n    read: 28\n    write: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /agencies\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agencies/{agency_key}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feed_versions\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feed_versions/export\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /feed_versions/{feed_version_key}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feed_versions/{feed_version_key}/download\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /feeds/{feed_key}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/{feed_key}/download_latest_feed_version\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /feeds/{feed_key}/download_latest_rt/{rt_type}.{format}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /onestop_id/{onestop_id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /operators\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /operators/{operator_key}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /routes\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /routes/{route_key}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /routes/{route_key}/trips\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /routes/{route_key}/trips/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /stops\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stops/{stop_key}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /stops/{stop_key}/departures\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /otp/plan\n  method: get\n  operationId: otpPlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /valhalla/centroid\n  method: get\n  operationId: valhallaCentroidGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /valhalla/centroid\n  method: post\n  operationId: valhallaCentroidPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /valhalla/expansion\n  method: get\n  operationId: valhallaExpansionGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /valhalla/expansion\n  method: post\n  operationId: valhallaExpansionPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /valhalla/isochrone\n  method: get\n  operationId:\
  \ valhallaIsochroneGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /valhalla/isochrone\n  method: post\n  operationId: valhallaIsochronePost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /valhalla/locate\n  method: get\n  operationId: valhallaLocateGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /valhalla/locate\n  method: post\n  operationId: valhallaLocatePost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /valhalla/optimized_route\n  method: get\n  operationId: valhallaOptimizedRouteGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /valhalla/optimized_route\n  method: post\n  operationId: valhallaOptimizedRoutePost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /valhalla/route\n  method: get\n  operationId: valhallaRouteGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /valhalla/route\n  method: post\n  operationId: valhallaRoutePost\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /valhalla/sources_to_targets\n  method: get\n  operationId: valhallaSourcesToTargetsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /valhalla/sources_to_targets\n  method: post\n  operationId: valhallaSourcesToTargetsPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /valhalla/trace_attributes\n  method: post\n  operationId: valhallaTraceAttributes\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /valhalla/trace_route\n  method: post\n  operationId: valhallaTraceRoute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/transitland/refs/heads/main/agentic-access/transitland-agentic-access.yml
summary_line: 37 operations · 9 acting
tags:
- Transportation
- Public APIs
- Transit
- GTFS
- Open Data
- Routing
- Geospatial
---
