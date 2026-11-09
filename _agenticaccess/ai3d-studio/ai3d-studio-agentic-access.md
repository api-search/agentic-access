---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 6
api_specs:
- filename: ai3d-studio-batches-api-openapi.yml
  format: yaml
  label: AI3D Studio Batches API
  slug: ai3d-studio-batches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai3d-studio/openapi/ai3d-studio-batches-api-openapi.yml
- filename: ai3d-studio-capabilities-api-openapi.yml
  format: yaml
  label: AI3D Studio Capabilities API
  slug: ai3d-studio-capabilities-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai3d-studio/openapi/ai3d-studio-capabilities-api-openapi.yml
- filename: ai3d-studio-generate-api-openapi.yml
  format: yaml
  label: AI3D Studio Generate API
  slug: ai3d-studio-generate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai3d-studio/openapi/ai3d-studio-generate-api-openapi.yml
- filename: ai3d-studio-health-api-openapi.yml
  format: yaml
  label: AI3D Studio Health API
  slug: ai3d-studio-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai3d-studio/openapi/ai3d-studio-health-api-openapi.yml
- filename: ai3d-studio-me-api-openapi.yml
  format: yaml
  label: AI3D Studio Me API
  slug: ai3d-studio-me-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai3d-studio/openapi/ai3d-studio-me-api-openapi.yml
- filename: ai3d-studio-quote-api-openapi.yml
  format: yaml
  label: AI3D Studio Quote API
  slug: ai3d-studio-quote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai3d-studio/openapi/ai3d-studio-quote-api-openapi.yml
- filename: ai3d-studio-tools-api-openapi.yml
  format: yaml
  label: AI3D Studio Tools API
  slug: ai3d-studio-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai3d-studio/openapi/ai3d-studio-tools-api-openapi.yml
- filename: ai3d-studio-workflows-api-openapi.yml
  format: yaml
  label: AI3D Studio Workflows API
  slug: ai3d-studio-workflows-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/ai3d-studio/openapi/ai3d-studio-workflows-api-openapi.yml
consequence_counts:
  read: 6
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ai3D Studio Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'AI3D Studio exposes 11 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AI3D Studio
provider_slug: ai3d-studio
slug: ai3d-studio-agentic-access
source_filename: ai3d-studio-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-01'\nmethod: generated\nsource: openapi/ai3d-studio-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    connected: 6\n    acting: 5\n  by_consequence:\n    read: 6\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /health\n  method: get\n  operationId: health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /capabilities\n  method: get\n  operationId:\
  \ getCapabilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /quote\n  method: post\n  operationId: quote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - read\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /generate\n  method: post\n  operationId: generate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - generate\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /batches\n  method: post\n  operationId: createBatch\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    scope:\n    - generate\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /batches\n  method: get\n  operationId: listBatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /batches/{id}\n  method: get\n  operationId: getBatch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /batches/{id}/retry\n  method: post\n  operationId: retryBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - generate\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n    \
  \  human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tools/convert\n  method: post\n  operationId: convertModel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - generate\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /workflows/{id}\n  method: get\n  operationId: getWorkflow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - read\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/ai3d-studio/agentic-access/ai3d-studio-agentic-access.yml
summary_line: 11 operations · 5 acting
tags:
- Artificial Intelligence
- 3D
- Generation
- Gaming
- 3D Printing
- Studio
---
