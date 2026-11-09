---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 1
api_specs:
- filename: buildonto-dev-batch-api-openapi.yml
  format: yaml
  label: Onto Batch API
  slug: buildonto-dev-batch-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildonto-dev/openapi/buildonto-dev-batch-api-openapi.yml
- filename: buildonto-dev-extract-api-openapi.yml
  format: yaml
  label: Onto Extract API
  slug: buildonto-dev-extract-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildonto-dev/openapi/buildonto-dev-extract-api-openapi.yml
- filename: buildonto-dev-map-api-openapi.yml
  format: yaml
  label: Onto Map API
  slug: buildonto-dev-map-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildonto-dev/openapi/buildonto-dev-map-api-openapi.yml
- filename: buildonto-dev-read-api-openapi.yml
  format: yaml
  label: Onto Read API
  slug: buildonto-dev-read-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildonto-dev/openapi/buildonto-dev-read-api-openapi.yml
- filename: buildonto-dev-read-score-api-openapi.yml
  format: yaml
  label: Onto Read + Score API
  slug: buildonto-dev-read-score-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildonto-dev/openapi/buildonto-dev-read-score-api-openapi.yml
- filename: buildonto-dev-score-api-openapi.yml
  format: yaml
  label: Onto Score API
  slug: buildonto-dev-score-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildonto-dev/openapi/buildonto-dev-score-api-openapi.yml
- filename: buildonto-dev-usage-api-openapi.yml
  format: yaml
  label: Onto Usage API
  slug: buildonto-dev-usage-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/buildonto-dev/openapi/buildonto-dev-usage-api-openapi.yml
consequence_counts:
  read: 1
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Buildonto Dev Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Onto exposes 7 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 read and 6 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Onto
provider_slug: buildonto-dev
slug: buildonto-dev-agentic-access
source_filename: buildonto-dev-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-03'\nmethod: generated\nsource: openapi/buildonto-dev-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    acting: 6\n    connected: 1\n  by_consequence:\n    write: 6\n    read: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/read\n  method: post\n  operationId: readUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/score\n  method: post\n  operationId: scoreUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/read-and-score\n  method: post\n  operationId: readAndScore\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/usage\n  method: get\n  operationId: getUsage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/batch\n  method: post\n  operationId: batch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/map\n  method: post\n  operationId: mapSite\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/extract\n  method: post\n  operationId: extract\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/buildonto-dev/agentic-access/buildonto-dev-agentic-access.yml
summary_line: 7 operations · 6 acting
tags:
- Artificial Intelligence
- Content
- Markdown
- Read API
- Platform
---
