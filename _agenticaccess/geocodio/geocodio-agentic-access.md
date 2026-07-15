---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 5
api_specs:
- filename: geocodio-openapi.yml
  format: yaml
  label: Geocodio Forward Geocoding
  slug: forward-geocoding
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geocodio/refs/heads/main/openapi/geocodio-openapi.yml
- filename: geocodio-openapi.yml
  format: yaml
  label: Geocodio Reverse Geocoding
  slug: reverse-geocoding
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geocodio/refs/heads/main/openapi/geocodio-openapi.yml
- filename: geocodio-openapi.yml
  format: yaml
  label: Geocodio Batch Geocoding
  slug: batch-geocoding
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geocodio/refs/heads/main/openapi/geocodio-openapi.yml
- filename: geocodio-openapi.yml
  format: yaml
  label: Geocodio Data Appends
  slug: data-appends
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geocodio/refs/heads/main/openapi/geocodio-openapi.yml
- filename: geocodio-openapi.yml
  format: yaml
  label: Geocodio Lists
  slug: lists
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/geocodio/refs/heads/main/openapi/geocodio-openapi.yml
consequence_counts:
  read: 5
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Geocodio Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Geocodio exposes 9 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Geocodio
provider_slug: geocodio
slug: geocodio-agentic-access
source_filename: geocodio-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/geocodio-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 5\n    acting: 4\n  by_consequence:\n    read: 5\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /geocode\n  method: get\n  operationId: geocode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geocode\n  method: post\n  operationId: batchGeocode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /reverse\n  method: get\n  operationId: reverse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reverse\n  method: post\n  operationId: batchReverse\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lists\n  method: get\n  operationId: listLists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lists\n  method: post\n  operationId: createList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lists/{id}\n  method: get\n  operationId: getList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lists/{id}\n  method: delete\n  operationId: deleteList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lists/{id}/download\n  method: get\n  operationId: downloadList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/geocodio/refs/heads/main/agentic-access/geocodio-agentic-access.yml
summary_line: 9 operations · 4 acting
tags:
- Geocoding
- Reverse Geocoding
- Addresses
- Data Append
- Census
---
