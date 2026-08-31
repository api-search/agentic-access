---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 8
api_specs:
- filename: sybilion-alerts-api-openapi.yml
  format: yaml
  label: Sybilion Alerts API
  slug: sybilion-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sybilion/refs/heads/main/openapi/sybilion-alerts-api-openapi.yml
- filename: sybilion-categories-api-openapi.yml
  format: yaml
  label: Sybilion Categories API
  slug: sybilion-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sybilion/refs/heads/main/openapi/sybilion-categories-api-openapi.yml
- filename: sybilion-drivers-api-openapi.yml
  format: yaml
  label: Sybilion Drivers API
  slug: sybilion-drivers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sybilion/refs/heads/main/openapi/sybilion-drivers-api-openapi.yml
- filename: sybilion-forecasts-api-openapi.yml
  format: yaml
  label: Sybilion Forecasts API
  slug: sybilion-forecasts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sybilion/refs/heads/main/openapi/sybilion-forecasts-api-openapi.yml
- filename: sybilion-health-api-openapi.yml
  format: yaml
  label: Sybilion Health API
  slug: sybilion-health-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sybilion/refs/heads/main/openapi/sybilion-health-api-openapi.yml
- filename: sybilion-jobs-api-openapi.yml
  format: yaml
  label: Sybilion Jobs API
  slug: sybilion-jobs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sybilion/refs/heads/main/openapi/sybilion-jobs-api-openapi.yml
- filename: sybilion-me-api-openapi.yml
  format: yaml
  label: Sybilion Me API
  slug: sybilion-me-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sybilion/refs/heads/main/openapi/sybilion-me-api-openapi.yml
- filename: sybilion-regions-api-openapi.yml
  format: yaml
  label: Sybilion Regions API
  slug: sybilion-regions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sybilion/refs/heads/main/openapi/sybilion-regions-api-openapi.yml
- filename: sybilion-usage-api-openapi.yml
  format: yaml
  label: Sybilion Usage API
  slug: sybilion-usage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sybilion/refs/heads/main/openapi/sybilion-usage-api-openapi.yml
consequence_counts:
  read: 8
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sybilion Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 11
overview: 'Sybilion exposes 11 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Sybilion
provider_slug: sybilion
slug: sybilion-agentic-access
source_filename: sybilion-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-11'\nmethod: generated\nsource: openapi/sybilion-operational-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 11\n  by_action_class:\n    acting: 3\n    connected: 8\n  by_consequence:\n    write: 3\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/alerts\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/categories\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/drivers\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/forecasts\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/forecasts/{id}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/forecasts/{id}/artifacts/{name}\n  method: get\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/jobs\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/me\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/regions\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/usage\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sybilion/refs/heads/main/agentic-access/sybilion-agentic-access.yml
summary_line: 11 operations · 3 acting
tags:
- Industrial market intelligence
- Commodity price forecasting
- Economic forecasting
- Time-series forecasting
- Procurement
- Supply-chain risk
- Trading analytics
- AI decision support
- MCP
- Agent-native
- Causal inference
- Anomaly detection
---
