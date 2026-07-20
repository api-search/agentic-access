---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 21
api_specs:
- filename: kadence-public-api-openapi.yml
  format: yaml
  label: Kadence Public API
  slug: kadence-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kadence/refs/heads/main/openapi/kadence-public-api-openapi.yml
consequence_counts:
  read: 21
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Kadence Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 27
overview: 'Kadence exposes 27 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Kadence
provider_slug: kadence
slug: kadence-agentic-access
source_filename: kadence-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/kadence-public-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 27\n  by_action_class:\n    connected: 21\n    acting: 6\n  by_consequence:\n    read: 21\n    write: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/public/bookable-days\n  method: get\n  operationId: api_v1publicbookable-days_get_collection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/bookable-days/{id}\n  method: get\n  operationId: api_v1publicbookable-days_id_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/public/bookable-onsite-passes\n  method: get\n  operationId: api_v1publicbookable-onsite-passes_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/bookable-spaces\n  method: get\n  operationId: api_v1publicbookable-spaces_get_collection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/bookings\n  method: get\n  operationId: api_v1publicbookings_get_collection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/bookings\n  method: post\n  operationId: api_v1publicbookings_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n  \
  \  token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public/bookings/{id}\n  method: get\n  operationId: api_v1publicbookings_id_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/bookings/{id}/cancel\n  method: post\n  operationId: api_v1publicbookings_idcancel_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public/bookings/{id}/check-in\n  method: post\n  operationId: api_v1publicbookings_idcheck-in_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public/bookings/{id}/check-out\n  method: post\n  operationId: api_v1publicbookings_idcheck-out_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public/users/{id}/bookings\n  method: get\n  operationId: api_v1publicusers_idbookings_get_collection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/buildings\n  method: get\n  operationId: api_v1publicbuildings_get_collection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/buildings/{id}\n  method: get\n  operationId: api_v1publicbuildings_id_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/floors\n  method: get\n  operationId: api_v1publicfloors_get_collection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/floors/{id}\n  method: get\n  operationId: api_v1publicfloors_id_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/neighborhoods\n  method: get\n  operationId: api_v1publicneighborhoods_get_collection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/public/neighborhoods/{id}\n  method: get\n  operationId: api_v1publicneighborhoods_id_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/spaces\n  method: get\n  operationId: api_v1publicspaces_get_collection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/spaces/{id}\n  method: get\n  operationId: api_v1publicspaces_id_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/users\n  method: get\n  operationId: api_v1publicusers_get_collection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/users/{id}\n\
  \  method: get\n  operationId: api_v1publicusers_id_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/users/{id}\n  method: patch\n  operationId: api_v1publicusers_id_patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public/users/{id}/photo\n  method: post\n  operationId: api_v1publicusers_idphoto_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public/visits\n  method: get\n  operationId:\
  \ api_v1publicvisits_get_collection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/visits/{id}\n  method: get\n  operationId: api_v1publicvisits_id_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/visitors\n  method: get\n  operationId: api_v1publicvisitors_get_collection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public/visitors/{id}\n  method: get\n  operationId: api_v1publicvisitors_id_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kadence/refs/heads/main/agentic-access/kadence-agentic-access.yml
summary_line: 27 operations · 6 acting
tags:
- Company
- Workplace
- Hybrid Work
- Desk Booking
- Room Booking
- Space Management
- Visitor Management
- Workplace Analytics
- Facilities
- OAuth
---
