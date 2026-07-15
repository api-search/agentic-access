---
acting_count: 0
action_class_counts:
  connected: 8
api_specs:
- filename: humboldt-universitat-zu-berlin-edoc-rest.yaml
  format: yaml
  label: edoc-Server DSpace REST API
  slug: edoc-rest
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/humboldt-universitat-zu-berlin/refs/heads/main/openapi/humboldt-universitat-zu-berlin-edoc-rest.yaml
consequence_counts:
  read: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Humboldt Universitat Zu Berlin Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Humboldt-Universität zu Berlin exposes 8 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Humboldt-Universität zu Berlin
provider_slug: humboldt-universitat-zu-berlin
slug: humboldt-universitat-zu-berlin-agentic-access
source_filename: humboldt-universitat-zu-berlin-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/humboldt-universitat-zu-berlin-edoc-rest.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 8\n  by_consequence:\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: getApiRoot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/communities\n  method: get\n  operationId: listCommunities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/communities/{uuid}\n  method: get\n  operationId:\
  \ getCommunity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/communities/{uuid}/collections\n  method: get\n  operationId: listCommunityCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/collections\n  method: get\n  operationId: listCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/collections/{uuid}\n  method: get\n  operationId: getCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/items/{uuid}\n  method: get\n  operationId: getItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /discover/search/objects\n  method: get\n  operationId: searchObjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/humboldt-universitat-zu-berlin/refs/heads/main/agentic-access/humboldt-universitat-zu-berlin-agentic-access.yml
summary_line: 8 operations
tags:
- Education
- Higher Education
- University
- Research
- Open Access
- Library
- Germany
---
