---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 5
api_specs:
- filename: blue-cheetah-blue-cheetah-api-api-openapi.yml
  format: yaml
  label: Blue Cheetah Blue Cheetah API
  slug: blue-cheetah-blue-cheetah-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blue-cheetah/openapi/blue-cheetah-blue-cheetah-api-api-openapi.yml
- filename: blue-cheetah-chat-api-openapi.yml
  format: yaml
  label: Blue Cheetah Chat API
  slug: blue-cheetah-chat-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blue-cheetah/openapi/blue-cheetah-chat-api-openapi.yml
- filename: blue-cheetah-completions-api-openapi.yml
  format: yaml
  label: Blue Cheetah Completions API
  slug: blue-cheetah-completions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blue-cheetah/openapi/blue-cheetah-completions-api-openapi.yml
- filename: blue-cheetah-health-api-openapi.yml
  format: yaml
  label: Blue Cheetah Health API
  slug: blue-cheetah-health-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blue-cheetah/openapi/blue-cheetah-health-api-openapi.yml
- filename: blue-cheetah-install-api-openapi.yml
  format: yaml
  label: Blue Cheetah Install API
  slug: blue-cheetah-install-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blue-cheetah/openapi/blue-cheetah-install-api-openapi.yml
- filename: blue-cheetah-metrics-api-openapi.yml
  format: yaml
  label: Blue Cheetah Metrics API
  slug: blue-cheetah-metrics-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blue-cheetah/openapi/blue-cheetah-metrics-api-openapi.yml
- filename: blue-cheetah-tt-pkg-key-api-openapi.yml
  format: yaml
  label: Blue Cheetah Tt Pkg Key API
  slug: blue-cheetah-tt-pkg-key-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blue-cheetah/openapi/blue-cheetah-tt-pkg-key-api-openapi.yml
consequence_counts:
  read: 5
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Blue Cheetah Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 7
overview: 'Blue Cheetah exposes 7 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 5 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Blue Cheetah
provider_slug: blue-cheetah
slug: blue-cheetah-agentic-access
source_filename: blue-cheetah-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-11-04'\nmethod: generated\nsource: openapi/blue-cheetah-blue-cheetah-api-api-openapi.yml, openapi/blue-cheetah-chat-api-openapi.yml,\n  openapi/blue-cheetah-completions-api-openapi.yml, openapi/blue-cheetah-health-api-openapi.yml,\n  openapi/blue-cheetah-install-api-openapi.yml, openapi/blue-cheetah-metrics-api-openapi.yml,\n  openapi/blue-cheetah-tt-pkg-key-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 7\n  by_action_class:\n    connected: 5\n    acting: 2\n  by_consequence:\n    read: 5\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /\n  method: get\n  operationId: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /chat\n  method: post\n  operationId: post_chat\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/completions\n  method: post\n  operationId: post_v1_completions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /health\n  method: get\n  operationId: get_health\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /install.sh\n  method: get\n  operationId: get_install_sh\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /metrics\n  method: get\n  operationId: get_metrics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tt-pkg-key.asc\n  method: get\n  operationId: get_tt_pkg_key_asc\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/blue-cheetah/agentic-access/blue-cheetah-agentic-access.yml
summary_line: 7 operations · 2 acting
tags:
- AI Hardware
- Compute
- Servers
- Workstations
---
