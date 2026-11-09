---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 12
api_specs:
- filename: 3dvalley-com-account-api-openapi.yml
  format: yaml
  label: 3D Valley Account API
  slug: 3dvalley-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/3dvalley-com/openapi/3dvalley-com-account-api-openapi.yml
- filename: 3dvalley-com-assets-api-openapi.yml
  format: yaml
  label: 3D Valley Assets API
  slug: 3dvalley-com-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/3dvalley-com/openapi/3dvalley-com-assets-api-openapi.yml
- filename: 3dvalley-com-categories-api-openapi.yml
  format: yaml
  label: 3D Valley Categories API
  slug: 3dvalley-com-categories-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/3dvalley-com/openapi/3dvalley-com-categories-api-openapi.yml
- filename: 3dvalley-com-jobs-api-openapi.yml
  format: yaml
  label: 3D Valley Jobs API
  slug: 3dvalley-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/3dvalley-com/openapi/3dvalley-com-jobs-api-openapi.yml
- filename: 3dvalley-com-tools-api-openapi.yml
  format: yaml
  label: 3D Valley Tools API
  slug: 3dvalley-com-tools-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/3dvalley-com/openapi/3dvalley-com-tools-api-openapi.yml
- filename: 3dvalley-com-uploads-api-openapi.yml
  format: yaml
  label: 3D Valley Uploads API
  slug: 3dvalley-com-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/3dvalley-com/openapi/3dvalley-com-uploads-api-openapi.yml
consequence_counts:
  read: 12
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: 3Dvalley Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: '3D Valley exposes 14 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: 3D Valley
provider_slug: 3dvalley-com
slug: 3dvalley-com-agentic-access
source_filename: 3dvalley-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/3dvalley-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 12\n    acting: 2\n  by_consequence:\n    read: 12\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /assets\n  method: get\n  operationId: searchAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/{id}\n  method: get\n  operationId: getAsset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/{id}/download\n  method: get\n  operationId:\
  \ downloadAsset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/{id}/preview\n  method: get\n  operationId: assetPreview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /categories\n  method: get\n  operationId: listCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tools\n  method: get\n  operationId: listTools\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs\n  method: post\n  operationId: createJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs\n  method: get\n  operationId: listJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{id}\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{id}/events\n  method: get\n  operationId: jobEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{id}/cancel\n  method: post\n  operationId: cancelJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /uploads\n  method: post\n  operationId: createUpload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/3dvalley-com/agentic-access/3dvalley-com-agentic-access.yml
summary_line: 14 operations · 2 acting
tags:
- AI Generation
- Texture Generation
- Asset Library
- Browser Tools
---
