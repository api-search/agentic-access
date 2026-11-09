---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 6
api_specs:
- filename: quady3d-com-account-api-openapi.yml
  format: yaml
  label: Quady3D AI Account API
  slug: quady3d-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quady3d-com/openapi/quady3d-com-account-api-openapi.yml
- filename: quady3d-com-assets-api-openapi.yml
  format: yaml
  label: Quady3D AI Assets API
  slug: quady3d-com-assets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quady3d-com/openapi/quady3d-com-assets-api-openapi.yml
- filename: quady3d-com-jobs-api-openapi.yml
  format: yaml
  label: Quady3D AI Jobs API
  slug: quady3d-com-jobs-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quady3d-com/openapi/quady3d-com-jobs-api-openapi.yml
- filename: quady3d-com-models-api-openapi.yml
  format: yaml
  label: Quady3D AI Models API
  slug: quady3d-com-models-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quady3d-com/openapi/quady3d-com-models-api-openapi.yml
- filename: quady3d-com-quotes-api-openapi.yml
  format: yaml
  label: Quady3D AI Quotes API
  slug: quady3d-com-quotes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quady3d-com/openapi/quady3d-com-quotes-api-openapi.yml
- filename: quady3d-com-uploads-api-openapi.yml
  format: yaml
  label: Quady3D AI Uploads API
  slug: quady3d-com-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quady3d-com/openapi/quady3d-com-uploads-api-openapi.yml
- filename: quady3d-com-open-api-api-openapi.yml
  format: yaml
  label: Quady3D AI Open API
  slug: quady3d-com-open-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/quady3d-com/openapi/quady3d-com-open-api-api-openapi.yml
consequence_counts:
  physical: 1
  read: 6
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Quady3D Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /uploads
operation_count: 9
overview: 'Quady3D AI exposes 9 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 2 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Quady3D AI
provider_slug: quady3d-com
slug: quady3d-com-agentic-access
source_filename: quady3d-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-05'\nmethod: generated\nsource: openapi/quady3d-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    connected: 6\n    acting: 3\n  by_consequence:\n    read: 6\n    physical: 1\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /models\n  method: get\n  operationId: listModels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /uploads\n  method: post\n  operationId:\
  \ uploadImage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /quotes\n  method: post\n  operationId: createQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /jobs\n  method: post\n  operationId: createJob\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n \
  \   audit: required\n- path: /jobs\n  method: get\n  operationId: listJobs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /jobs/{id}\n  method: get\n  operationId: getJob\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/{id}\n  method: get\n  operationId: downloadAsset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi\n  method: get\n  operationId: getOpenApi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/quady3d-com/agentic-access/quady3d-com-agentic-access.yml
summary_line: 9 operations · 3 acting
tags:
- Company
- Artificial Intelligence
- 3D
- Generation
- Image
- Text
---
