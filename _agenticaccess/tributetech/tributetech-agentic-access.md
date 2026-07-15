---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 5
api_specs:
- filename: tributetech-openapi.yml
  format: yaml
  label: Tribute Store Authentication API
  slug: tributetech-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tributetech/refs/heads/main/openapi/tributetech-openapi.yml
- filename: tributetech-openapi.yml
  format: yaml
  label: Tribute Store Serving Locations API
  slug: tributetech-serving-locations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tributetech/refs/heads/main/openapi/tributetech-openapi.yml
- filename: tributetech-openapi.yml
  format: yaml
  label: Tribute Store Obituaries API
  slug: tributetech-obituaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tributetech/refs/heads/main/openapi/tributetech-openapi.yml
consequence_counts:
  read: 5
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tributetech Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Tribute Technology exposes 8 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Tribute Technology
provider_slug: tributetech
slug: tributetech-agentic-access
source_filename: tributetech-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/tributetech-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 3\n    connected: 5\n  by_consequence:\n    write: 3\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /token/\n  method: post\n  operationId: createToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/external-location/post\n  method: post\n  operationId: postExternalLocation\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/locations/{servingLocationId}\n  method: get\n  operationId: getLocation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/locations/\n  method: get\n  operationId: listLocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/locations/getlocationtypes\n  method: get\n  operationId: getLocationTypes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/external-case/post\n  method: post\n  operationId: postExternalCase\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/obituaries/GetObituary/{obituaryId}\n  method: get\n  operationId: getObituary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/obituaries\n  method: get\n  operationId: listObituaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tributetech/refs/heads/main/agentic-access/tributetech-agentic-access.yml
summary_line: 8 operations · 3 acting
tags:
- Funeral Technology
- Obituaries
- Memorials
- Funeral Homes
- E-commerce
- Death Care
- Case Management
---
