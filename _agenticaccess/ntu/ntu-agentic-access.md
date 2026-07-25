---
acting_count: 0
action_class_counts:
  connected: 6
api_specs:
- filename: ntu-discover-api-openapi.yml
  format: yaml
  label: Nanyang Technological University Discover API
  slug: ntu-discover-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntu/refs/heads/main/openapi/ntu-discover-api-openapi.yml
- filename: ntu-info-api-openapi.yml
  format: yaml
  label: Nanyang Technological University Info API
  slug: ntu-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntu/refs/heads/main/openapi/ntu-info-api-openapi.yml
- filename: ntu-items-api-openapi.yml
  format: yaml
  label: Nanyang Technological University Items API
  slug: ntu-items-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntu/refs/heads/main/openapi/ntu-items-api-openapi.yml
- filename: ntu-oai-pmh-api-openapi.yml
  format: yaml
  label: Nanyang Technological University OAI-PMH API
  slug: ntu-oai-pmh-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntu/refs/heads/main/openapi/ntu-oai-pmh-api-openapi.yml
- filename: ntu-root-api-openapi.yml
  format: yaml
  label: Nanyang Technological University Root API
  slug: ntu-root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntu/refs/heads/main/openapi/ntu-root-api-openapi.yml
- filename: ntu-search-api-openapi.yml
  format: yaml
  label: Nanyang Technological University Search API
  slug: ntu-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ntu/refs/heads/main/openapi/ntu-search-api-openapi.yml
consequence_counts:
  read: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ntu Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Nanyang Technological University exposes 6 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Nanyang Technological University
provider_slug: ntu
slug: ntu-agentic-access
source_filename: ntu-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/ntu-drntu-data.yaml, openapi/ntu-drntu-repo-oai.yaml, openapi/ntu-drntu-repo-rest.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 6\n  by_consequence:\n    read: 6\n  human_in_the_loop_required: 0\noperations:\n- path: /info/version\n  method: get\n  operationId: getVersion\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /search\n  method: get\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /request\n  method:\
  \ get\n  operationId: oaiRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: getApiRoot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /discover/search/objects\n  method: get\n  operationId: discoverSearchObjects\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /core/items/{uuid}\n  method: get\n  operationId: getItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ntu/refs/heads/main/agentic-access/ntu-agentic-access.yml
summary_line: 6 operations
tags:
- Education
- Higher Education
- University
- Singapore
- Research Data
- Open Data
- Repository
- Library
---
