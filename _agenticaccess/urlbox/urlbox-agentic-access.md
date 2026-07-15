---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 3
api_specs:
- filename: urlbox-openapi.yml
  format: yaml
  label: Urlbox Synchronous Render API
  slug: urlbox-render-sync-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urlbox/refs/heads/main/openapi/urlbox-openapi.yml
- filename: urlbox-openapi.yml
  format: yaml
  label: Urlbox Asynchronous Render API
  slug: urlbox-render-async-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urlbox/refs/heads/main/openapi/urlbox-openapi.yml
- filename: urlbox-openapi.yml
  format: yaml
  label: Urlbox Render Status API
  slug: urlbox-render-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urlbox/refs/heads/main/openapi/urlbox-openapi.yml
- filename: urlbox-openapi.yml
  format: yaml
  label: Urlbox Render Links API
  slug: urlbox-render-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urlbox/refs/heads/main/openapi/urlbox-openapi.yml
- filename: urlbox-openapi.yml
  format: yaml
  label: Urlbox Webhooks API
  slug: urlbox-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urlbox/refs/heads/main/openapi/urlbox-openapi.yml
- filename: urlbox-openapi.yml
  format: yaml
  label: Urlbox Usage API
  slug: urlbox-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/urlbox/refs/heads/main/openapi/urlbox-openapi.yml
consequence_counts:
  read: 3
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Urlbox Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 5
overview: 'Urlbox exposes 5 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Urlbox
provider_slug: urlbox
slug: urlbox-agentic-access
source_filename: urlbox-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/urlbox-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 5\n  by_action_class:\n    acting: 2\n    connected: 3\n  by_consequence:\n    write: 2\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /render/sync\n  method: post\n  operationId: createSyncRender\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /render/async\n  method: post\n  operationId: createAsyncRender\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /render/{renderId}\n  method: get\n  operationId: getRenderStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{apiKey}/{token}/{format}\n  method: get\n  operationId: getRenderLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/urlbox/refs/heads/main/agentic-access/urlbox-agentic-access.yml
summary_line: 5 operations · 2 acting
tags:
- Screenshots
- Rendering
- PDF
- Video
- Web Capture
---
