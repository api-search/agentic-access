---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: openapi.yml
  format: yaml
  label: medRxiv REST API
  slug: medrxiv-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/medrxiv/refs/heads/main/openapi/openapi.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Medrxiv Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'medRxiv exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: medRxiv
provider_slug: medrxiv
slug: medrxiv-agentic-access
source_filename: medrxiv-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /details/{server}/{interval}/{cursor}/{format}\n  method: get\n  operationId: getDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /details/{server}/{doi}/na/{format}\n  method: get\n  operationId: getDetailsByDoi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pubs/{server}/{interval}/{cursor}\n\
  \  method: get\n  operationId: getPublications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pubs/{server}/{doi}/na/{format}\n  method: get\n  operationId: getPublicationByDoi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /usage/{interval}/{server}/{format}\n  method: get\n  operationId: getUsageStatistics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/medrxiv/refs/heads/main/agentic-access/medrxiv-agentic-access.yml
summary_line: 5 operations
tags:
- Health Sciences
- Preprints
- Research
- Open Access
- Medical Research
- Clinical Research
- Scientific Publications
---
