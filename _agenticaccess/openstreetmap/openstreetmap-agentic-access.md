---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 10
api_specs:
- filename: openstreetmap-main-openapi.yml
  format: yaml
  label: OpenStreetMap Main Editing API v0.6
  slug: main-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstreetmap/refs/heads/main/openapi/openstreetmap-main-openapi.yml
- filename: openstreetmap-nominatim-openapi.yml
  format: yaml
  label: OpenStreetMap Nominatim Geocoding API
  slug: nominatim-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openstreetmap/refs/heads/main/openapi/openstreetmap-nominatim-openapi.yml
consequence_counts:
  read: 10
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Openstreetmap Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 18
overview: 'OpenStreetMap exposes 18 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: OpenStreetMap
provider_slug: openstreetmap
slug: openstreetmap-agentic-access
source_filename: openstreetmap-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openstreetmap-main-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 18\n  by_action_class:\n    connected: 10\n    acting: 8\n  by_consequence:\n    read: 10\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /map\n  method: get\n  operationId: getMapData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read_prefs\n    - write_api\n    - write_notes\n- path: /node/{id}\n  method: get\n  operationId: getNode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n    scope:\n    - read_prefs\n    - write_api\n    - write_notes\n- path: /node/{id}\n  method: put\n  operationId: updateNode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read_prefs\n    - write_api\n    - write_notes\n- path: /node/{id}\n  method: delete\n  operationId: deleteNode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read_prefs\n    - write_api\n    - write_notes\n- path: /node/create\n  method: put\n  operationId: createNode\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read_prefs\n    - write_api\n    - write_notes\n- path: /node/{id}/{version}\n  method: get\n  operationId: getNodeVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read_prefs\n    - write_api\n    - write_notes\n- path: /way/{id}\n  method: get\n  operationId: getWay\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read_prefs\n    - write_api\n    - write_notes\n- path: /relation/{id}\n  method: get\n  operationId: getRelation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read_prefs\n    - write_api\n    - write_notes\n- path: /changeset/create\n  method: put\n  operationId: createChangeset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read_prefs\n    - write_api\n    - write_notes\n- path: /changeset/{id}\n  method: get\n  operationId: getChangeset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read_prefs\n    - write_api\n    - write_notes\n- path: /changeset/{id}\n  method: put\n  operationId: updateChangeset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read_prefs\n    - write_api\n    - write_notes\n- path: /changeset/{id}/close\n  method: put\n  operationId: closeChangeset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read_prefs\n    - write_api\n    - write_notes\n- path: /changeset/{id}/upload\n  method: post\n  operationId: uploadChangeset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n    scope:\n    - read_prefs\n    - write_api\n    - write_notes\n- path: /notes\n  method: get\n  operationId: searchNotes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read_prefs\n    - write_api\n    - write_notes\n- path: /notes\n  method: post\n  operationId: createNote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - read_prefs\n    - write_api\n    - write_notes\n- path: /notes/{id}\n  method: get\n  operationId: getNote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read_prefs\n    - write_api\n\
  \    - write_notes\n- path: /user/details\n  method: get\n  operationId: getUserDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read_prefs\n    - write_api\n    - write_notes\n- path: /capabilities\n  method: get\n  operationId: getCapabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - read_prefs\n    - write_api\n    - write_notes\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openstreetmap/refs/heads/main/agentic-access/openstreetmap-agentic-access.yml
summary_line: 18 operations · 8 acting
tags:
- Geospatial
- Mapping
- Open Data
- Geocoding
- Editing
---
