---
acting_count: 0
action_class_counts:
  connected: 9
api_specs:
- filename: national-energy-system-operator-openapi.json
  format: json
  label: NESO Data Portal API
  slug: data-portal-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/national-energy-system-operator/main/openapi/national-energy-system-operator-openapi.json
consequence_counts:
  read: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: National Energy System Operator Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'National Energy System Operator exposes 9 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: National Energy System Operator
provider_slug: national-energy-system-operator
slug: national-energy-system-operator-agentic-access
source_filename: national-energy-system-operator-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/national-energy-system-operator-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 9\n  by_consequence:\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /organization_list\n  method: get\n  operationId: organizationList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /package_list\n  method: get\n  operationId: packageList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tag_list\n  method: get\n  operationId:\
  \ tagList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /package_search\n  method: get\n  operationId: packageSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource_search\n  method: get\n  operationId: resourceSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /package_show\n  method: get\n  operationId: packageShow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource_show\n  method: get\n  operationId: resourceShow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /datastore_search\n  method: get\n  operationId: datastoreSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /datastore_search_sql\n  method: get\n  operationId: datastoreSearchSql\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/national-energy-system-operator/refs/heads/main/agentic-access/national-energy-system-operator-agentic-access.yml
summary_line: 9 operations
tags:
- Energy
- Electricity
- Grid
- Open Data
- United Kingdom
---
