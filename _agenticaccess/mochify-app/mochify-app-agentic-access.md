---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 2
api_specs:
- filename: mochify-app-generate-api-openapi.yml
  format: yaml
  label: mochify-app Generate API
  slug: mochify-app-generate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mochify-app/openapi/mochify-app-generate-api-openapi.yml
- filename: mochify-app-image-api-openapi.yml
  format: yaml
  label: mochify-app Image API
  slug: mochify-app-image-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mochify-app/openapi/mochify-app-image-api-openapi.yml
- filename: mochify-app-meta-api-openapi.yml
  format: yaml
  label: mochify-app Meta API
  slug: mochify-app-meta-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mochify-app/openapi/mochify-app-meta-api-openapi.yml
- filename: mochify-app-pdf-api-openapi.yml
  format: yaml
  label: mochify-app PDF API
  slug: mochify-app-pdf-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mochify-app/openapi/mochify-app-pdf-api-openapi.yml
- filename: mochify-app-upload-api-openapi.yml
  format: yaml
  label: mochify-app Upload API
  slug: mochify-app-upload-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/mochify-app/openapi/mochify-app-upload-api-openapi.yml
consequence_counts:
  read: 2
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Mochify App Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'mochify-app exposes 8 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: mochify-app
provider_slug: mochify-app
slug: mochify-app-agentic-access
source_filename: mochify-app-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/mochify-app-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 6\n    connected: 2\n  by_consequence:\n    write: 6\n    read: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/squish\n  method: post\n  operationId: squishImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/checkTokens\n  method: get\n  operationId: checkTokens\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/pdf\n  method: post\n  operationId: processPdf\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/generate\n  method: post\n  operationId: generateImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/upload/init\n  method: post\n  operationId: initUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/upload/chunk\n  method: post\n  operationId: uploadChunk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/upload/complete\n  method: post\n  operationId: completeUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /health\n  method: get\n  operationId: healthCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n"
source_yaml_url: https://artifacts.apis.io/mochify-app/agentic-access/mochify-app-agentic-access.yml
summary_line: 8 operations · 6 acting
tags:
- Company
- Image Compression
- Video Compression
- PDF compression
- Artificial Intelligence
- PrivacyFocused
---
