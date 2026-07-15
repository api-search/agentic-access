---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 10
api_specs:
- filename: vesselfinder-ais-api-openapi.yml
  format: yaml
  label: VesselFinder AIS API
  slug: vesselfinder-ais-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vesselfinder/refs/heads/main/openapi/vesselfinder-ais-api-openapi.yml
- filename: vesselfinder-container-tracking-api-openapi.yml
  format: yaml
  label: VesselFinder Container Tracking API
  slug: vesselfinder-container-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vesselfinder/refs/heads/main/openapi/vesselfinder-container-tracking-api-openapi.yml
consequence_counts:
  read: 10
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Vesselfinder Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 13
overview: 'VesselFinder exposes 13 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: VesselFinder
provider_slug: vesselfinder
slug: vesselfinder-agentic-access
source_filename: vesselfinder-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/vesselfinder-ais-api-openapi.yml, openapi/vesselfinder-container-tracking-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    connected: 10\n    acting: 3\n  by_consequence:\n    read: 10\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /vessels\n  method: get\n  operationId: getVessels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portcalls\n  method: get\n  operationId: getPortCalls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /expectedarrivals\n  method: get\n  operationId: getExpectedArrivals\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /masterdata\n  method: get\n  operationId: getMasterData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /distance\n  method: get\n  operationId: getDistance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /vesselslist\n  method: get\n  operationId: getVesselsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /livedata\n  method: get\n  operationId: getLiveData\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /listmanager\n  method: get\n  operationId: getWatchlist\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /listmanager\n  method: post\n  operationId: addWatchlistVessels\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listmanager\n  method: put\n  operationId: replaceWatchlistVessels\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n   \
  \ subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /listmanager\n  method: delete\n  operationId: deleteWatchlistVessels\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /container/{apiKey}/{containerNumber}/{sealine}\n  method: get\n  operationId: trackContainer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vesselfinder/refs/heads/main/agentic-access/vesselfinder-agentic-access.yml
summary_line: 13 operations · 3 acting
tags:
- AIS
- Maritime
- Vessel Tracking
- Container Tracking
- Geospatial
- Logistics
- Ports
- Supply Chain
---
