---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 5
api_specs:
- filename: snipe-it-file-api-openapi.yml
  format: yaml
  label: Snipe-IT File API
  slug: snipe-it-file-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snipe-it/openapi/snipe-it-file-api-openapi.yml
- filename: snipe-it-files-api-openapi.yml
  format: yaml
  label: Snipe-IT Files API
  slug: snipe-it-files-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snipe-it/openapi/snipe-it-files-api-openapi.yml
- filename: snipe-it-hardware-api-openapi.yml
  format: yaml
  label: Snipe-IT Hardware API
  slug: snipe-it-hardware-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snipe-it/openapi/snipe-it-hardware-api-openapi.yml
- filename: snipe-it-models-api-openapi.yml
  format: yaml
  label: Snipe-IT Models API
  slug: snipe-it-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snipe-it/openapi/snipe-it-models-api-openapi.yml
- filename: snipe-it-snipe-it-api-api-openapi.yml
  format: yaml
  label: Snipe-IT Snipe IT API
  slug: snipe-it-snipe-it-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/snipe-it/openapi/snipe-it-snipe-it-api-api-openapi.yml
consequence_counts:
  read: 5
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Snipe It Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Snipe-IT exposes 7 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Snipe-IT
provider_slug: snipe-it
slug: snipe-it-agentic-access
source_filename: snipe-it-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/snipe-it-file-api-openapi.yml, openapi/snipe-it-files-api-openapi.yml, openapi/snipe-it-hardware-api-openapi.yml,\n  openapi/snipe-it-models-api-openapi.yml, openapi/snipe-it-snipe-it-api-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 5\n    acting: 2\n  by_consequence:\n    read: 5\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/{v1id}/1/file/1\n  method: get\n  operationId: get_api_v1_v1id_1_file_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/{v1id}/1/files\n  method: get\n  operationId:\
  \ get_api_v1_v1id_1_files\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/hardware\n  method: get\n  operationId: get_api_v1_hardware\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/hardware/1/files/1/delete\n  method: delete\n  operationId: delete_api_v1_hardware_1_files_1_delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/hardware/1/{1Id}/1\n  method: get\n  operationId: get_api_v1_hardware_1_1Id_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/v1/models/1/file/1\n  method: delete\n  operationId: delete_api_v1_models_1_file_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /\n  method: get\n  operationId: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/snipe-it/agentic-access/snipe-it-agentic-access.yml
summary_line: 7 operations · 2 acting
tags:
- IT Asset Management
- Open Source
- Cloud Hosting
- REST API
- Security
- Support
- Software
---
