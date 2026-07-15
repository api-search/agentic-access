---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 4
api_specs:
- filename: revolutio-hazard-api-openapi.yml
  format: yaml
  label: Revolutio Hazard API
  slug: revolutio-hazard-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/revolutio/refs/heads/main/openapi/revolutio-hazard-api-openapi.yml
consequence_counts:
  read: 4
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Revolutio Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'Revolutio exposes 8 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 4 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Revolutio
provider_slug: revolutio
slug: revolutio-agentic-access
source_filename: revolutio-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/revolutio-hazard-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    connected: 4\n    acting: 4\n  by_consequence:\n    read: 4\n    write: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /asnzs1170/wind\n  method: get\n  operationId: getWindHazardGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asnzs1170/wind\n  method: post\n  operationId: getWindHazardPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n    \
  \  human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asnzs1170/snow\n  method: get\n  operationId: getSnowHazardGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asnzs1170/snow\n  method: post\n  operationId: getSnowHazardPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asnzs1170/seismic\n  method: get\n  operationId: getSeismicHazardGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asnzs1170/seismic\n  method: post\n  operationId: getSeismicHazardPost\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /asnzs1170/combined\n  method: get\n  operationId: getCombinedHazardGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /asnzs1170/combined\n  method: post\n  operationId: getCombinedHazardPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/revolutio/refs/heads/main/agentic-access/revolutio-agentic-access.yml
summary_line: 8 operations · 4 acting
tags:
- Engineering
- Hazard
- Weather
- Structural Engineering
- Wind Analysis
- Construction
---
