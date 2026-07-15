---
acting_count: 0
action_class_counts:
  connected: 8
api_specs:
- filename: aoc-data-api.yaml
  format: yaml
  label: Architect of the Capitol Data API
  slug: aoc-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/architect-of-the-capitol/refs/heads/main/openapi/aoc-data-api.yaml
consequence_counts:
  read: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Architect Of The Capitol Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Architect of the Capitol exposes 8 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Architect of the Capitol
provider_slug: architect-of-the-capitol
slug: architect-of-the-capitol-agentic-access
source_filename: architect-of-the-capitol-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/aoc-data-api.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 8\n  by_consequence:\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /buildings\n  method: get\n  operationId: listBuildings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /buildings/{buildingId}\n  method: get\n  operationId: getBuilding\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artworks\n  method: get\n  operationId: listArtworks\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /artworks/{artworkId}\n  method: get\n  operationId: getArtwork\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /preservation-projects\n  method: get\n  operationId: listPreservationProjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /preservation-projects/{projectId}\n  method: get\n  operationId: getPreservationProject\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /visitor-info\n  method: get\n  operationId: getVisitorInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /accessibility\n  method: get\n  operationId: getAccessibilityInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/architect-of-the-capitol/refs/heads/main/agentic-access/architect-of-the-capitol-agentic-access.yml
summary_line: 8 operations
tags:
- Federal Government
- Capitol Hill
- Congress
- Historic Preservation
- Government Services
---
