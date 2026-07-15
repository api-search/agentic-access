---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 3
api_specs:
- filename: kpler-openapi.yml
  format: yaml
  label: Kpler Liquids API
  slug: kpler-liquids-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kpler/refs/heads/main/openapi/kpler-openapi.yml
- filename: kpler-openapi.yml
  format: yaml
  label: Kpler LNG API
  slug: kpler-lng-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kpler/refs/heads/main/openapi/kpler-openapi.yml
- filename: kpler-openapi.yml
  format: yaml
  label: Kpler LPG API
  slug: kpler-lpg-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kpler/refs/heads/main/openapi/kpler-openapi.yml
- filename: kpler-openapi.yml
  format: yaml
  label: Kpler Dry Bulk API
  slug: kpler-dry-bulk-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kpler/refs/heads/main/openapi/kpler-openapi.yml
- filename: kpler-openapi.yml
  format: yaml
  label: Kpler Freight API
  slug: kpler-freight-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/kpler/refs/heads/main/openapi/kpler-openapi.yml
consequence_counts:
  read: 3
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Kpler Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 4
overview: 'Kpler exposes 4 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Kpler
provider_slug: kpler
slug: kpler-agentic-access
source_filename: kpler-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/kpler-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    acting: 1\n    connected: 3\n  by_consequence:\n    write: 1\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /login\n  method: post\n  operationId: login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/trades\n  method: get\n  operationId: getTrades\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/flows\n  method: get\n  operationId: getFlows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/vessels\n  method: get\n  operationId: getVessels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/kpler/refs/heads/main/agentic-access/kpler-agentic-access.yml
summary_line: 4 operations · 1 acting
tags:
- Vessel Tracking
- Maritime
- Commodities
- Supply Chain
- AIS
- Trade Flows
- Shipping
- Energy
---
