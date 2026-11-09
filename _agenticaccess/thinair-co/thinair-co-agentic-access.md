---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 19
api_specs:
- filename: thinair-co-account-api-openapi.yml
  format: yaml
  label: thinair-co Account API
  slug: thinair-co-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thinair-co/openapi/thinair-co-account-api-openapi.yml
- filename: thinair-co-billing-api-openapi.yml
  format: yaml
  label: thinair-co Billing API
  slug: thinair-co-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thinair-co/openapi/thinair-co-billing-api-openapi.yml
- filename: thinair-co-conditions-api-openapi.yml
  format: yaml
  label: thinair-co Conditions API
  slug: thinair-co-conditions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thinair-co/openapi/thinair-co-conditions-api-openapi.yml
- filename: thinair-co-connections-api-openapi.yml
  format: yaml
  label: thinair-co Connections API
  slug: thinair-co-connections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thinair-co/openapi/thinair-co-connections-api-openapi.yml
- filename: thinair-co-geocoding-api-openapi.yml
  format: yaml
  label: thinair-co Geocoding API
  slug: thinair-co-geocoding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thinair-co/openapi/thinair-co-geocoding-api-openapi.yml
- filename: thinair-co-geofences-api-openapi.yml
  format: yaml
  label: thinair-co Geofences API
  slug: thinair-co-geofences-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thinair-co/openapi/thinair-co-geofences-api-openapi.yml
- filename: thinair-co-intersections-api-openapi.yml
  format: yaml
  label: thinair-co Intersections API
  slug: thinair-co-intersections-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thinair-co/openapi/thinair-co-intersections-api-openapi.yml
- filename: thinair-co-learning-api-openapi.yml
  format: yaml
  label: thinair-co Learning API
  slug: thinair-co-learning-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thinair-co/openapi/thinair-co-learning-api-openapi.yml
- filename: thinair-co-migrations-api-openapi.yml
  format: yaml
  label: thinair-co Migrations API
  slug: thinair-co-migrations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thinair-co/openapi/thinair-co-migrations-api-openapi.yml
- filename: thinair-co-places-api-openapi.yml
  format: yaml
  label: thinair-co Places API
  slug: thinair-co-places-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thinair-co/openapi/thinair-co-places-api-openapi.yml
- filename: thinair-co-query-api-openapi.yml
  format: yaml
  label: thinair-co Query API
  slug: thinair-co-query-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thinair-co/openapi/thinair-co-query-api-openapi.yml
- filename: thinair-co-routing-api-openapi.yml
  format: yaml
  label: thinair-co Routing API
  slug: thinair-co-routing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thinair-co/openapi/thinair-co-routing-api-openapi.yml
- filename: thinair-co-tables-api-openapi.yml
  format: yaml
  label: thinair-co Tables API
  slug: thinair-co-tables-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/thinair-co/openapi/thinair-co-tables-api-openapi.yml
consequence_counts:
  read: 19
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Thinair Co Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 34
overview: 'thinair-co exposes 34 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 19 read and 15 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: thinair-co
provider_slug: thinair-co
slug: thinair-co-agentic-access
source_filename: thinair-co-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/data-thinair-co-openapi.json, openapi/geo-thinair-co-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 34\n  by_action_class:\n    connected: 19\n    acting: 15\n  by_consequence:\n    read: 19\n    write: 15\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/tables/{t}/profile\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tables/{t}/anomalies\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/query/optimize\n  method:\
  \ post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/migrations/generate\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/quota\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connections\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connections/{id}/health\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connections/{id}/schema\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/query\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/query/history\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/weather\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/traffic\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/explore\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/places\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/isochrone\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/geocode\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/place\n  method: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/autocomplete\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reverse\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/directions\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/locate\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/quota\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/intersection\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/intersections/search\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/distance-matrix\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v1/geofences/contains\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/geofences/validate\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/search/structured\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/batch\n\
  \  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/geocode/batch\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/map-match\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/trace-attributes\n  method: post\n  x-agentic-access:\n  \
  \  action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/feedback\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /geo/feedback\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/thinair-co/agentic-access/thinair-co-agentic-access.yml
summary_line: 34 operations · 15 acting
tags:
- Company
- Fleet Management
- Telematics
- Logistics
- Compliance
---
