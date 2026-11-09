---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 3
api_specs:
- filename: usefomo-applications-api-openapi.yml
  format: yaml
  label: FOMO Applications API
  slug: usefomo-applications-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/usefomo/openapi/usefomo-applications-api-openapi.yml
consequence_counts:
  read: 3
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Usefomo Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 8
overview: 'FOMO exposes 8 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 5 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: FOMO
provider_slug: usefomo
slug: usefomo-agentic-access
source_filename: usefomo-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-26'\nmethod: generated\nsource: openapi/usefomo-api-settings-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 8\n  by_action_class:\n    acting: 5\n    connected: 3\n  by_consequence:\n    write: 5\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /applications/me/:ID\n  method: patch\n  operationId: update-application\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/me/dashboard?date_range[from]=2020-03-20&date_range[to]=2020-04-20\n  method:\
  \ get\n  operationId: application-get-statistics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/me/event_types\n  method: post\n  operationId: create-a-template\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/me/events\n  method: post\n  operationId: create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/me/events/:ID\n  method: get\n  operationId: get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/me/events/:ID\n  method: patch\n  operationId: update-event\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/me/events/:ID\n  method: delete\n  operationId: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/me/events/find\n  method: get\n  operationId: search-for-an-event\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/usefomo/agentic-access/usefomo-agentic-access.yml
summary_line: 8 operations · 5 acting
tags:
- Company
- Social Proof
- Marketing
- Software-as-a-Service
- E-Commerce
---
