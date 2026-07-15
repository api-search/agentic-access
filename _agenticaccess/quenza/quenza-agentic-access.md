---
acting_count: 8
action_class_counts:
  acting: 8
  connected: 4
api_specs:
- filename: quenza-openapi.yml
  format: yaml
  label: Quenza Clients API
  slug: quenza-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-openapi.yml
- filename: quenza-openapi.yml
  format: yaml
  label: Quenza Groups API
  slug: quenza-groups-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-openapi.yml
- filename: quenza-openapi.yml
  format: yaml
  label: Quenza Members API
  slug: quenza-members-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-openapi.yml
- filename: quenza-openapi.yml
  format: yaml
  label: Quenza Tasks API
  slug: quenza-tasks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/openapi/quenza-openapi.yml
consequence_counts:
  read: 4
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Quenza Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 12
overview: 'Quenza exposes 12 API operations that an AI agent could call, of which 8 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 8 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Quenza
provider_slug: quenza
slug: quenza-agentic-access
source_filename: quenza-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/quenza-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 12\n  by_action_class:\n    connected: 4\n    acting: 8\n  by_consequence:\n    read: 4\n    write: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /clients\n  method: get\n  operationId: developers.v1.clients.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clients\n  method: post\n  operationId: developers.v1.clients.create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clients/{client}\n  method: get\n  operationId: developers.v1.clients.show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clients/{client}\n  method: patch\n  operationId: developers.v1.clients.update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clients/{client}/archive\n  method: post\n  operationId: developers.v1.clients.archive\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /clients/{client}/unarchive\n  method: post\n  operationId: developers.v1.clients.unarchive\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups\n  method: post\n  operationId: developers.v1.groups.create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /groups/{group}/members\n  method: post\n  operationId: developers.v1.groups.members.attach\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /members\n  method: get\n  operationId: developers.v1.members.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /members\n  method: post\n  operationId: developers.v1.members.create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /members/{professional}\n  method: patch\n  operationId: developers.v1.members.update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tasks\n  method: get\n  operationId: developers.v1.tasks.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/quenza/refs/heads/main/agentic-access/quenza-agentic-access.yml
summary_line: 12 operations · 8 acting
tags:
- Coaching
- Therapy
- Client Engagement
- Digital Health
- Mental Health
- Practice Management
- Positive Psychology
---
