---
acting_count: 0
action_class_counts:
  connected: 5
api_specs:
- filename: tenderapi-eu-organisations-api-openapi.yml
  format: yaml
  label: tenderapi-eu Organisations API
  slug: tenderapi-eu-organisations-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tenderapi-eu/openapi/tenderapi-eu-organisations-api-openapi.yml
- filename: tenderapi-eu-tenders-api-openapi.yml
  format: yaml
  label: tenderapi-eu Tenders API
  slug: tenderapi-eu-tenders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/tenderapi-eu/openapi/tenderapi-eu-tenders-api-openapi.yml
consequence_counts:
  read: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tenderapi Eu Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'tenderapi-eu exposes 5 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: tenderapi-eu
provider_slug: tenderapi-eu
slug: tenderapi-eu-agentic-access
source_filename: tenderapi-eu-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/tenderapi-eu-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    connected: 5\n  by_consequence:\n    read: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /tenders/search\n  method: post\n  operationId: searchTenders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tenders/{id}\n  method: get\n  operationId: getTender\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organisations/search\n  method: post\n  operationId: searchOrganisations\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organisations/{id}\n  method: get\n  operationId: getOrganisation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /organisations/{id}/tenders\n  method: get\n  operationId: getOrganisationTenders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/tenderapi-eu/agentic-access/tenderapi-eu-agentic-access.yml
summary_line: 5 operations
tags:
- EU
- Procurement
- Tenders
- Data
---
