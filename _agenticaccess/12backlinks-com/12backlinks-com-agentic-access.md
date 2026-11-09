---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 7
api_specs:
- filename: 12backlinks-com-account-api-openapi.yml
  format: yaml
  label: 12backlinks Account API
  slug: 12backlinks-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/12backlinks-com/openapi/12backlinks-com-account-api-openapi.yml
- filename: 12backlinks-com-analyses-api-openapi.yml
  format: yaml
  label: 12backlinks Analyses API
  slug: 12backlinks-com-analyses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/12backlinks-com/openapi/12backlinks-com-analyses-api-openapi.yml
- filename: 12backlinks-com-batches-api-openapi.yml
  format: yaml
  label: 12backlinks Batches API
  slug: 12backlinks-com-batches-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/12backlinks-com/openapi/12backlinks-com-batches-api-openapi.yml
- filename: 12backlinks-com-link-gaps-api-openapi.yml
  format: yaml
  label: 12backlinks Link Gaps API
  slug: 12backlinks-com-link-gaps-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/12backlinks-com/openapi/12backlinks-com-link-gaps-api-openapi.yml
- filename: 12backlinks-com-markets-api-openapi.yml
  format: yaml
  label: 12backlinks Markets API
  slug: 12backlinks-com-markets-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/12backlinks-com/openapi/12backlinks-com-markets-api-openapi.yml
consequence_counts:
  read: 7
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: 12Backlinks Com Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 10
overview: '12backlinks exposes 10 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: 12backlinks
provider_slug: 12backlinks-com
slug: 12backlinks-com-agentic-access
source_filename: 12backlinks-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/12backlinks-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 10\n  by_action_class:\n    connected: 7\n    acting: 3\n  by_consequence:\n    read: 7\n    write: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/markets\n  method: get\n  operationId: list_markets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/account\n  method: get\n  operationId: get_account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/batches\n  method: post\n\
  \  operationId: analyze_keywords\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/batches\n  method: get\n  operationId: list_batches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/batches/{id}\n  method: get\n  operationId: get_batch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/analyses/{id}\n  method: get\n  operationId: get_analysis\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/link-gaps/quote\n  method:\
  \ post\n  operationId: quote_link_gap\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/link-gaps\n  method: post\n  operationId: launch_link_gap\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/link-gaps\n  method: get\n  operationId: list_link_gaps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/link-gaps/{id}\n  method: get\n  operationId: get_link_gap\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/12backlinks-com/agentic-access/12backlinks-com-agentic-access.yml
summary_line: 10 operations · 3 acting
tags:
- SEO
- Backlinks
- Marketing
- French
---
