---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 4
api_specs:
- filename: docling-cli-openapi.yml
  format: yaml
  label: Docling Python Library
  slug: docling-python-library
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docling/refs/heads/main/openapi/docling-cli-openapi.yml
- filename: docling-serve-openapi.yml
  format: yaml
  label: Docling Serve REST API
  slug: docling-serve-rest-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/docling/refs/heads/main/openapi/docling-serve-openapi.yml
consequence_counts:
  read: 4
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Docling Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 9
overview: 'Docling exposes 9 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Docling
provider_slug: docling
slug: docling-agentic-access
source_filename: docling-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/docling-cli-openapi.yml, openapi/docling-serve-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    acting: 5\n    connected: 4\n  by_consequence:\n    write: 5\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/convert\n  method: post\n  operationId: cliConvert\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/convert/source\n  method: post\n  operationId: convertSource\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/convert/file\n  method: post\n  operationId: convertFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/convert/source/async\n  method: post\n  operationId: convertSourceAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/convert/file/async\n \
  \ method: post\n  operationId: convertFileAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/status/poll/{task_id}\n  method: get\n  operationId: pollTaskStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/result/{task_id}\n  method: get\n  operationId: getTaskResult\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: getHealth\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi.json\n\
  \  method: get\n  operationId: getOpenApiSpec\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/docling/refs/heads/main/agentic-access/docling-agentic-access.yml
summary_line: 9 operations · 5 acting
tags:
- Documents
- Parsing
- PDF
- OCR
- Layout
- Tables
- RAG
- LLM
- Open Source
- IBM Research
- LF AI and Data
- MCP
- Knowledge Graph
- Generative AI
---
