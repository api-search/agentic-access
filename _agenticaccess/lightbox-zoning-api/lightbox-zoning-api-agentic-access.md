---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 2
api_specs:
- filename: lightbox-zoning-api-openapi.yml
  format: yaml
  label: LightBox Zoning API
  slug: lightbox-zoning-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lightbox-zoning-api/refs/heads/main/openapi/lightbox-zoning-api-openapi.yml
consequence_counts:
  read: 2
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Lightbox Zoning Api Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 3
overview: 'LightBox Zoning API exposes 3 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: LightBox Zoning API
provider_slug: lightbox-zoning-api
slug: lightbox-zoning-api-agentic-access
source_filename: lightbox-zoning-api-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/lightbox-zoning-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 3\n  by_action_class:\n    connected: 2\n    acting: 1\n  by_consequence:\n    read: 2\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /zoning/us/parcel/{parcelId}\n  method: get\n  operationId: getZoningByParcel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /zoning/us/address\n  method: get\n  operationId: getZoningByAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /zoning/us/geometry\n  method: post\n  operationId: getZoningByGeometry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lightbox-zoning-api/refs/heads/main/agentic-access/lightbox-zoning-api-agentic-access.yml
summary_line: 3 operations · 1 acting
tags:
- Zoning
- Real Estate
- CRE
- Property
- Parcels
- Geospatial
- Land Use
---
