---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 3
api_specs:
- filename: fabtally-com-attest-api-openapi.yml
  format: yaml
  label: fabtally-com Attest API
  slug: fabtally-com-attest-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabtally-com/openapi/fabtally-com-attest-api-openapi.yml
- filename: fabtally-com-dfm-api-openapi.yml
  format: yaml
  label: fabtally-com DFM API
  slug: fabtally-com-dfm-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabtally-com/openapi/fabtally-com-dfm-api-openapi.yml
- filename: fabtally-com-discovery-api-openapi.yml
  format: yaml
  label: fabtally-com Discovery API
  slug: fabtally-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabtally-com/openapi/fabtally-com-discovery-api-openapi.yml
- filename: fabtally-com-quote-api-openapi.yml
  format: yaml
  label: fabtally-com Quote API
  slug: fabtally-com-quote-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabtally-com/openapi/fabtally-com-quote-api-openapi.yml
- filename: fabtally-com-slice-api-openapi.yml
  format: yaml
  label: fabtally-com Slice API
  slug: fabtally-com-slice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/fabtally-com/openapi/fabtally-com-slice-api-openapi.yml
consequence_counts:
  read: 3
  write: 11
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fabtally Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 14
overview: 'fabtally-com exposes 14 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 11 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: fabtally-com
provider_slug: fabtally-com
slug: fabtally-com-agentic-access
source_filename: fabtally-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/fabtally-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 14\n  by_action_class:\n    connected: 3\n    acting: 11\n  by_consequence:\n    read: 3\n    write: 11\n  human_in_the_loop_required: 0\noperations:\n- path: /agent/overview\n  method: get\n  operationId: overview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/v1/quote\n  method: post\n  operationId: quote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/v1/analyze\n  method: post\n  operationId: analyze\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/v1/preview\n  method: post\n  operationId: preview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/v1/slice\n  method: post\n  operationId: slice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/v1/slice/preview\n  method: post\n  operationId: slice_preview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/v1/slice/gcode\n  method: post\n  operationId: slice_gcode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/v1/slice/full\n  method: post\n  operationId: slice_full\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/v1/dfm-preview\n  method: post\n  operationId: dfm_preview\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/v1/dfm\n  method: post\n  operationId: dfm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/v1/orient\n  method: post\n  operationId: orient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n \
  \   audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/v1/attest/schema\n  method: get\n  operationId: attest_schema\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /agent/v1/attest\n  method: post\n  operationId: attest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /agent/health\n  method: get\n  operationId: health_check\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/fabtally-com/agentic-access/fabtally-com-agentic-access.yml
summary_line: 14 operations · 11 acting
tags:
- Company
- 3D Printing
- Slicing
- Quotes
- Manufacturing
---
