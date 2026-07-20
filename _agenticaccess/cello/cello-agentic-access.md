---
acting_count: 3
action_class_counts:
  acting: 3
  connected: 3
api_specs:
- filename: cello-openapi-original.json
  format: json
  label: Cello API
  slug: cello-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cello/refs/heads/main/openapi/cello-openapi-original.json
consequence_counts:
  read: 3
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cello Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'Cello exposes 6 API operations that an AI agent could call, of which 3 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read and 3 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cello
provider_slug: cello
slug: cello-agentic-access
source_filename: cello-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/cello-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 3\n    connected: 3\n  by_consequence:\n    write: 3\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /token\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /referral-codes/{code}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n  \
  \    max-ttl: 3600\n    audit: none\n- path: /new-users/{productUserId}/reward\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /referral-codes/active-link/{productUserId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /referrers/{productUserId}/depersonalize\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cello/refs/heads/main/agentic-access/cello-agentic-access.yml
summary_line: 6 operations · 3 acting
tags:
- Company
- Referral Marketing
- Affiliate Marketing
- Growth
- SaaS
- Attribution
- Partner Programs
- Ai Enterprise Software
---
