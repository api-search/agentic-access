---
acting_count: 0
action_class_counts:
  connected: 12
api_specs:
- filename: cutluma-com-cutluma-public-api-api-openapi.yml
  format: yaml
  label: CutLuma CutLuma Public API
  slug: cutluma-com-cutluma-public-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cutluma-com/openapi/cutluma-com-cutluma-public-api-api-openapi.yml
- filename: cutluma-com-llms-full-txt-api-openapi.yml
  format: yaml
  label: CutLuma Llms Full.txt API
  slug: cutluma-com-llms-full-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cutluma-com/openapi/cutluma-com-llms-full-txt-api-openapi.yml
- filename: cutluma-com-llms-txt-api-openapi.yml
  format: yaml
  label: CutLuma Llms.txt API
  slug: cutluma-com-llms-txt-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cutluma-com/openapi/cutluma-com-llms-txt-api-openapi.yml
- filename: cutluma-com-oembed-api-openapi.yml
  format: yaml
  label: CutLuma Oembed API
  slug: cutluma-com-oembed-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cutluma-com/openapi/cutluma-com-oembed-api-openapi.yml
- filename: cutluma-com-public-api-openapi.yml
  format: yaml
  label: CutLuma Public API
  slug: cutluma-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/cutluma-com/openapi/cutluma-com-public-api-openapi.yml
consequence_counts:
  read: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cutluma Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'CutLuma exposes 12 API operations that an AI agent could call, of which 0 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CutLuma
provider_slug: cutluma-com
slug: cutluma-com-agentic-access
source_filename: cutluma-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/cutluma-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 12\n  by_consequence:\n    read: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /api/public/catalog\n  method: get\n  operationId: catalog\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public/search\n  method: get\n  operationId: search\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public/templates\n  method: get\n  operationId: templates\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public/plans\n  method: get\n  operationId: plans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public/playbooks\n  method: get\n  operationId: playbooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public/sizes\n  method: get\n  operationId: sizes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/public/editor-link\n  method: get\n  operationId: editorLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/public/{token}\n  method: get\n  operationId: sharedVideo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/oembed\n  method: get\n  operationId: oembed\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms.txt\n  method: get\n  operationId: llms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms-full.txt\n  method: get\n  operationId: llmsFull\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{hub}/{slug}.md\n  method: get\n  operationId: pageMarkdown\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/cutluma-com/agentic-access/cutluma-com-agentic-access.yml
summary_line: 12 operations
tags:
- Video Editing
- Artificial Intelligence
- Free
- Online
- Multilingual
- Company
---
