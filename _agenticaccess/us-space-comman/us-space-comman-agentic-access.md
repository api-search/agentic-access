---
acting_count: 1
action_class_counts:
  acting: 1
  connected: 7
api_specs:
- filename: us-space-command-space-track-openapi.yml
  format: yaml
  label: Space-Track.org REST API
  slug: space-track-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/us-space-comman/refs/heads/main/openapi/us-space-command-space-track-openapi.yml
consequence_counts:
  read: 7
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Us Space Comman Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'US Space Command exposes 8 API operations that an AI agent could call, of which 1 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read and 1 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: US Space Command
provider_slug: us-space-comman
slug: us-space-comman-agentic-access
source_filename: us-space-comman-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/us-space-command-space-track-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 1\n    connected: 7\n  by_consequence:\n    write: 1\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /ajaxauth/login\n  method: post\n  operationId: login\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /basicspacedata/query/class/gp/format/{format}\n  method: get\n  operationId: listCurrentGP\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /basicspacedata/query/class/satcat/format/{format}\n  method: get\n  operationId: listSatCat\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /basicspacedata/query/class/cdm_public/format/{format}\n  method: get\n  operationId: listConjunctionData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /basicspacedata/query/class/decay/format/{format}\n  method: get\n  operationId: listDecayData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /basicspacedata/query/class/tip/format/{format}\n  method: get\n  operationId: listTrackingImpactPredictions\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /basicspacedata/query/class/gp_history/format/{format}\n  method: get\n  operationId: listGPHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /basicspacedata/query/class/boxscore/format/{format}\n  method: get\n  operationId: getBoxscore\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/us-space-comman/refs/heads/main/agentic-access/us-space-comman-agentic-access.yml
summary_line: 8 operations · 1 acting
tags:
- Federal Government
- Space
- Space Situational Awareness
- Satellite Tracking
- Open Data
---
