---
acting_count: 0
action_class_counts:
  connected: 6
api_specs:
- filename: mcgill-dataverse-native.yaml
  format: yaml
  label: McGill University Dataverse (Borealis) - Native API
  slug: dataverse-native
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mcgill/refs/heads/main/openapi/mcgill-dataverse-native.yaml
- filename: mcgill-dataverse-search.yaml
  format: yaml
  label: McGill University Dataverse (Borealis) - Search API
  slug: dataverse-search
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/mcgill/refs/heads/main/openapi/mcgill-dataverse-search.yaml
consequence_counts:
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Mcgill Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'McGill University exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: McGill University
provider_slug: mcgill
slug: mcgill-agentic-access
source_filename: mcgill-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/mcgill-dataverse-native.yaml, openapi/mcgill-dataverse-search.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 6\n  by_consequence:\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /dataverses/{identifier}\n  method: get\n  operationId: Dataverses_getDataverse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dataverses/{identifier}/contents\n  method: get\n  operationId: Dataverses_listContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /info/version\n  method: get\n  operationId: Info_getInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /info/metrics/dataverses\n  method: get\n  operationId: Metrics_getDataversesAllTime\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method: get\n  operationId: Search_search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search/services\n  method: get\n  operationId: Search_getSearchEngines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/mcgill/refs/heads/main/agentic-access/mcgill-agentic-access.yml
summary_line: 6 operations
tags:
- Education
- Higher Education
- University
- Research Data
- Open Data
- Canada
- Quebec
---
