---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 3
api_specs:
- filename: openapi.yaml
  format: yaml
  label: Valhalla Route API
  slug: valhalla-route-api
  spec_type: OpenAPI
  url: https://valhalla.github.io/valhalla/api/openapi/
- filename: openapi.yaml
  format: yaml
  label: Valhalla Optimized Route API
  slug: valhalla-optimized-route-api
  spec_type: OpenAPI
  url: https://valhalla.github.io/valhalla/api/openapi/
- filename: openapi.yaml
  format: yaml
  label: Valhalla Matrix API
  slug: valhalla-matrix-api
  spec_type: OpenAPI
  url: https://valhalla.github.io/valhalla/api/openapi/
- filename: openapi.yaml
  format: yaml
  label: Valhalla Isochrone API
  slug: valhalla-isochrone-api
  spec_type: OpenAPI
  url: https://valhalla.github.io/valhalla/api/openapi/
- filename: openapi.yaml
  format: yaml
  label: Valhalla Map Matching API
  slug: valhalla-map-matching-api
  spec_type: OpenAPI
  url: https://valhalla.github.io/valhalla/api/openapi/
- filename: openapi.yaml
  format: yaml
  label: Valhalla Elevation API
  slug: valhalla-elevation-api
  spec_type: OpenAPI
  url: https://valhalla.github.io/valhalla/api/openapi/
- filename: openapi.yaml
  format: yaml
  label: Valhalla Expansion API
  slug: valhalla-expansion-api
  spec_type: OpenAPI
  url: https://valhalla.github.io/valhalla/api/openapi/
- filename: openapi.yaml
  format: yaml
  label: Valhalla Locate API
  slug: valhalla-locate-api
  spec_type: OpenAPI
  url: https://valhalla.github.io/valhalla/api/openapi/
- filename: openapi.yaml
  format: yaml
  label: Valhalla Status API
  slug: valhalla-status-api
  spec_type: OpenAPI
  url: https://valhalla.github.io/valhalla/api/openapi/
consequence_counts:
  read: 3
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Valhalla Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Valhalla exposes 12 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 9 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Valhalla
provider_slug: valhalla
slug: valhalla-agentic-access
source_filename: valhalla-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    acting: 9\n    connected: 3\n  by_consequence:\n    write: 9\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /route\n  method: post\n  operationId: route\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /optimized_route\n  method: post\n  operationId: optimizedRoute\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sources_to_targets\n  method: post\n  operationId: sourcesToTargets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /isochrone\n  method: post\n  operationId: isochrone\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /trace_route\n  method: post\n  operationId: traceRoute\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /trace_attributes\n  method: post\n  operationId: traceAttributes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /height\n  method: post\n  operationId: height\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /locate\n  method: get\n  operationId: locateGet\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /locate\n  method: post\n  operationId: locate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /expansion\n  method: post\n  operationId: expansion\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /status\n  method: get\n  operationId: status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tile/{z}/{x}/{y}.mvt\n\
  \  method: get\n  operationId: tile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/valhalla/refs/heads/main/agentic-access/valhalla-agentic-access.yml
summary_line: 12 operations · 9 acting
tags:
- Routing
- Navigation
- OpenStreetMap
- Mapping
- Geospatial
- Directions
- Isochrones
- Travel
- Transportation
- Open Source
---
