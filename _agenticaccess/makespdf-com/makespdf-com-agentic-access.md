---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 3
api_specs:
- filename: makespdf-com-artifacts-api-openapi.yml
  format: yaml
  label: makespdf-com Artifacts API
  slug: makespdf-com-artifacts-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makespdf-com/openapi/makespdf-com-artifacts-api-openapi.yml
- filename: makespdf-com-public-api-openapi.yml
  format: yaml
  label: makespdf-com Public API
  slug: makespdf-com-public-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makespdf-com/openapi/makespdf-com-public-api-openapi.yml
- filename: makespdf-com-render-api-openapi.yml
  format: yaml
  label: makespdf-com Render API
  slug: makespdf-com-render-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makespdf-com/openapi/makespdf-com-render-api-openapi.yml
- filename: makespdf-com-validate-api-openapi.yml
  format: yaml
  label: makespdf-com Validate API
  slug: makespdf-com-validate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makespdf-com/openapi/makespdf-com-validate-api-openapi.yml
- filename: makespdf-com-x402-api-openapi.yml
  format: yaml
  label: makespdf-com X402 API
  slug: makespdf-com-x402-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/makespdf-com/openapi/makespdf-com-x402-api-openapi.yml
consequence_counts:
  read: 3
  safety-critical: 1
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Makespdf Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/canvas
operation_count: 10
overview: 'makespdf-com exposes 10 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read, 6 write, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: makespdf-com
provider_slug: makespdf-com
slug: makespdf-com-agentic-access
source_filename: makespdf-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/makespdf-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    acting: 7\n    connected: 3\n  by_consequence:\n    write: 6\n    safety-critical: 1\n    read: 3\n  human_in_the_loop_required: 1\noperations:\n- path: /api/v1/markdown\n  method: post\n  operationId: markdownToPdf\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/render\n  method: post\n  operationId: renderPdf\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/md\n  method: post\n  operationId: mdToPdf\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/canvas\n  method: post\n  operationId: canvasToPdf\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/preview\n  method: post\n\
  \  operationId: previewPdf\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/templates\n  method: get\n  operationId: listTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/templates/{id}\n  method: get\n  operationId: getTemplate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/artifacts\n  method: get\n  operationId: listArtifacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/md/validate\n  method:\
  \ post\n  operationId: validateMarkdown\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/preview/validate\n  method: post\n  operationId: validateTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/makespdf-com/agentic-access/makespdf-com-agentic-access.yml
summary_line: 10 operations · 7 acting · 1 human-in-the-loop
tags:
- Company
- PDF
- Conversion
- Developers
---
