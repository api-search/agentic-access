---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 8
api_specs:
- filename: filetypeconverters-com-batches-api-openapi.yml
  format: yaml
  label: FileType Converters Batches API
  slug: filetypeconverters-com-batches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filetypeconverters-com/openapi/filetypeconverters-com-batches-api-openapi.yml
- filename: filetypeconverters-com-convert-api-openapi.yml
  format: yaml
  label: FileType Converters Convert API
  slug: filetypeconverters-com-convert-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filetypeconverters-com/openapi/filetypeconverters-com-convert-api-openapi.yml
- filename: filetypeconverters-com-formats-api-openapi.yml
  format: yaml
  label: FileType Converters Formats API
  slug: filetypeconverters-com-formats-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filetypeconverters-com/openapi/filetypeconverters-com-formats-api-openapi.yml
- filename: filetypeconverters-com-jobs-api-openapi.yml
  format: yaml
  label: FileType Converters Jobs API
  slug: filetypeconverters-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filetypeconverters-com/openapi/filetypeconverters-com-jobs-api-openapi.yml
- filename: filetypeconverters-com-openapi-json-api-openapi.yml
  format: yaml
  label: FileType Converters Openapi.json API
  slug: filetypeconverters-com-openapi-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filetypeconverters-com/openapi/filetypeconverters-com-openapi-json-api-openapi.yml
- filename: filetypeconverters-com-pairs-api-openapi.yml
  format: yaml
  label: FileType Converters Pairs API
  slug: filetypeconverters-com-pairs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filetypeconverters-com/openapi/filetypeconverters-com-pairs-api-openapi.yml
- filename: filetypeconverters-com-usage-api-openapi.yml
  format: yaml
  label: FileType Converters Usage API
  slug: filetypeconverters-com-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/filetypeconverters-com/openapi/filetypeconverters-com-usage-api-openapi.yml
consequence_counts:
  read: 8
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Filetypeconverters Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: 'FileType Converters exposes 10 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: FileType Converters
provider_slug: filetypeconverters-com
slug: filetypeconverters-com-agentic-access
source_filename: filetypeconverters-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-07'\nmethod: generated\nsource: openapi/filetypeconverters-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 2\n    connected: 8\n  by_consequence:\n    write: 2\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/convert\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/pairs\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/v1/formats\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/jobs/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/jobs/{id}/download\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/batches\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/batches/{id}\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/batches/{id}/download\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/usage\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/openapi.json\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/filetypeconverters-com/agentic-access/filetypeconverters-com-agentic-access.yml
summary_line: 10 operations · 2 acting
tags:
- File Conversion
- Document Conversion
- PDF
- OCR
- Spreadsheets
- Images
- MCP
- Developer API
- AI Deep Read
- File Formats
---
