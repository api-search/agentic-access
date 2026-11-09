---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 3
api_specs:
- filename: dynamoi-com-data-api-openapi.yml
  format: yaml
  label: Dynamoi Data API
  slug: dynamoi-com-data-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/dynamoi-com/openapi/dynamoi-com-data-api-openapi.yml
consequence_counts:
  physical: 1
  read: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dynamoi Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/data/v1/checkout
operation_count: 4
overview: 'Dynamoi exposes 4 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Dynamoi
provider_slug: dynamoi-com
slug: dynamoi-com-agentic-access
source_filename: dynamoi-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-06'\nmethod: generated\nsource: openapi/dynamoi-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    connected: 3\n    acting: 1\n  by_consequence:\n    read: 3\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/data/mpp/v1/catalog\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/mpp/v1/bundles/snapshot\n  method: get\n  operationId: getMusicRoyaltiesSnapshotBundle\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/data/v1/checkout\n\
  \  method: post\n  operationId: createDataCheckoutSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/data/v1/publications/{publicationId}\n  method: get\n  operationId: getPaidDataPublication\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/dynamoi-com/agentic-access/dynamoi-com-agentic-access.yml
summary_line: 4 operations · 1 acting
tags:
- Music Promotion
- Spotify
- YouTube
- Distribution
- Analytics
- Independent Artists
- Labels
---
