---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 4
api_specs:
- filename: vite-javascript-api-openapi.yml
  format: yaml
  label: Vite JavaScript API
  slug: javascript-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vite/refs/heads/main/openapi/vite-javascript-api-openapi.yml
- filename: vite-plugin-api-openapi.yml
  format: yaml
  label: Vite Plugin API
  slug: plugin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/vite/refs/heads/main/openapi/vite-plugin-api-openapi.yml
consequence_counts:
  read: 4
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Vite Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Vite exposes 6 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Vite
provider_slug: vite
slug: vite-agentic-access
source_filename: vite-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/vite-javascript-api-openapi.yml, openapi/vite-plugin-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 4\n    acting: 2\n  by_consequence:\n    read: 4\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /__vite_ping\n  method: get\n  operationId: pingDevServer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /@vite/client\n  method: get\n  operationId: getViteClient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /@fs/{filePath}\n  method: get\n  operationId: serveFileSystemFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /__open-in-editor\n  method: get\n  operationId: openInEditor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /__hmr/update\n  method: post\n  operationId: triggerHmrUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /__hmr/full-reload\n  method: post\n  operationId: triggerFullReload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/vite/refs/heads/main/agentic-access/vite-agentic-access.yml
summary_line: 6 operations · 2 acting
tags:
- Build Tools
- Bundler
- Development Server
- ESM
- Frontend
- Hot Module Replacement
- JavaScript
- Plugin API
- TypeScript
- Vite
---
