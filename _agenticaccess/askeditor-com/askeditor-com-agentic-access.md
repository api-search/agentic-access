---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 3
api_specs:
- filename: askeditor-com-estimate-api-openapi.yml
  format: yaml
  label: AskEditor Estimate API
  slug: askeditor-com-estimate-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/askeditor-com/openapi/askeditor-com-estimate-api-openapi.yml
- filename: askeditor-com-recipes-api-openapi.yml
  format: yaml
  label: AskEditor Recipes API
  slug: askeditor-com-recipes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/askeditor-com/openapi/askeditor-com-recipes-api-openapi.yml
- filename: askeditor-com-run-api-openapi.yml
  format: yaml
  label: AskEditor Run API
  slug: askeditor-com-run-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/askeditor-com/openapi/askeditor-com-run-api-openapi.yml
- filename: askeditor-com-uploads-api-openapi.yml
  format: yaml
  label: AskEditor Uploads API
  slug: askeditor-com-uploads-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/askeditor-com/openapi/askeditor-com-uploads-api-openapi.yml
consequence_counts:
  read: 3
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Askeditor Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'AskEditor exposes 6 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AskEditor
provider_slug: askeditor-com
slug: askeditor-com-agentic-access
source_filename: askeditor-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-02'\nmethod: generated\nsource: openapi/askeditor-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    connected: 3\n    acting: 3\n  by_consequence:\n    read: 3\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/recipes\n  method: get\n  operationId: listTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/estimate\n  method: get\n  operationId: estimate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/uploads\n  method: post\n  operationId:\
  \ createUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/uploads/{ticket}/file\n  method: post\n  operationId: uploadFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/uploads/{ticket}\n  method: get\n  operationId: getUpload\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/run/remove-background\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/askeditor-com/agentic-access/askeditor-com-agentic-access.yml
summary_line: 6 operations · 3 acting
tags:
- Artificial Intelligence
- Video Editing
- Automation
- Productivity
---
