---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 8
api_specs:
- filename: bee-maps-account-api-openapi.yml
  format: yaml
  label: Bee Maps Account API
  slug: bee-maps-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bee-maps/refs/heads/main/openapi/bee-maps-account-api-openapi.yml
- filename: bee-maps-ai-events-api-openapi.yml
  format: yaml
  label: Bee Maps AI Events API
  slug: bee-maps-ai-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bee-maps/refs/heads/main/openapi/bee-maps-ai-events-api-openapi.yml
- filename: bee-maps-bursts-api-openapi.yml
  format: yaml
  label: Bee Maps Bursts API
  slug: bee-maps-bursts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bee-maps/refs/heads/main/openapi/bee-maps-bursts-api-openapi.yml
- filename: bee-maps-devices-api-openapi.yml
  format: yaml
  label: Bee Maps Devices API
  slug: bee-maps-devices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bee-maps/refs/heads/main/openapi/bee-maps-devices-api-openapi.yml
- filename: bee-maps-imagery-api-openapi.yml
  format: yaml
  label: Bee Maps Imagery API
  slug: bee-maps-imagery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bee-maps/refs/heads/main/openapi/bee-maps-imagery-api-openapi.yml
- filename: bee-maps-map-features-api-openapi.yml
  format: yaml
  label: Bee Maps Map Features API
  slug: bee-maps-map-features-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bee-maps/refs/heads/main/openapi/bee-maps-map-features-api-openapi.yml
consequence_counts:
  read: 8
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bee Maps Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Bee Maps exposes 9 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Bee Maps
provider_slug: bee-maps
slug: bee-maps-agentic-access
source_filename: bee-maps-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-27'\nmethod: generated\nsource: openapi/openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 8\n    acting: 1\n  by_consequence:\n    read: 8\n    write: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /latest/poly\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /map-data\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /burst/create\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bursts\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /aievents/search\n  method: post\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /aievents/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /balance\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /history\n  method: get\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /devices\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bee-maps/refs/heads/main/agentic-access/bee-maps-agentic-access.yml
summary_line: 9 operations · 1 acting
tags:
- Company
- Mapping
- GIS
- Location
- Data
---
