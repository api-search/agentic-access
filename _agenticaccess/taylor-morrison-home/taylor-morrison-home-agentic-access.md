---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 10
api_specs:
- filename: taylor-morrison-home-search-openapi.yml
  format: yaml
  label: Taylor Morrison Home Search API
  slug: taylor-morrison-home-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/taylor-morrison-home/refs/heads/main/openapi/taylor-morrison-home-search-openapi.yml
consequence_counts:
  read: 10
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Taylor Morrison Home Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'taylor-morrison-home exposes 11 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: taylor-morrison-home
provider_slug: taylor-morrison-home
slug: taylor-morrison-home-agentic-access
source_filename: taylor-morrison-home-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/taylor-morrison-home-search-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 10\n    acting: 1\n  by_consequence:\n    read: 10\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /communities\n  method: get\n  operationId: listCommunities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /communities/{community_id}\n  method: get\n  operationId: getCommunity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /homes\n\
  \  method: get\n  operationId: listHomes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /homes/{home_id}\n  method: get\n  operationId: getHome\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /floor-plans\n  method: get\n  operationId: listFloorPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /floor-plans/{plan_id}\n  method: get\n  operationId: getFloorPlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lots\n  method: get\n  operationId: listLots\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /reservations\n  method: post\n  operationId: createReservation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reservations\n  method: get\n  operationId: listReservations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reservations/{reservation_id}\n  method: get\n  operationId: getReservation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /design/options\n  method: get\n  operationId: listDesignOptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/taylor-morrison-home/refs/heads/main/agentic-access/taylor-morrison-home-agentic-access.yml
summary_line: 11 operations · 1 acting
tags:
- Homebuilding
- Real Estate
- Fortune 1000
- New Homes
- Communities
- Mortgage
---
