---
acting_count: 4
action_class_counts:
  acting: 4
api_specs:
- filename: indieml-app-keys-api-openapi.yml
  format: yaml
  label: indieml-app Keys API
  slug: indieml-app-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indieml-app/openapi/indieml-app-keys-api-openapi.yml
- filename: indieml-app-score-api-openapi.yml
  format: yaml
  label: indieml-app Score API
  slug: indieml-app-score-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/indieml-app/openapi/indieml-app-score-api-openapi.yml
consequence_counts:
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Indieml App Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'indieml-app exposes 4 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: indieml-app
provider_slug: indieml-app
slug: indieml-app-agentic-access
source_filename: indieml-app-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/indieml-app-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    acting: 4\n  by_consequence:\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/score/substance\n  method: post\n  operationId: score_text_v1_score_substance_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/score/substance/batch\n  method: post\n  operationId: score_text_batch_v1_score_substance_batch_post\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/score/demo\n  method: post\n  operationId: score_demo_v1_score_demo_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/keys/generate\n  method: post\n  operationId: generate_key_v1_keys_generate_post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/indieml-app/agentic-access/indieml-app-agentic-access.yml
summary_line: 4 operations · 4 acting
tags:
- Artificial Intelligence
- Natural Language Processing
- Text Analysis
- Machine Learning
---
