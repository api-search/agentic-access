---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 4
api_specs:
- filename: ourpeople-openapi.yml
  format: yaml
  label: OurPeople API
  slug: ourpeople-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/ourpeople/refs/heads/main/openapi/ourpeople-openapi.yml
consequence_counts:
  read: 4
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Ourpeople Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 6
overview: 'OurPeople exposes 6 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read and 2 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: OurPeople
provider_slug: ourpeople
slug: ourpeople-agentic-access
source_filename: ourpeople-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/ourpeople-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 2\n    connected: 4\n  by_consequence:\n    write: 2\n    read: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/auth\n  method: post\n  operationId: createToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/refresh\n  method: post\n  operationId: refreshToken\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/broadcasts/deliveries\n  method: get\n  operationId: listDeliveries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/broadcasts/{broadcastId}\n  method: get\n  operationId: getBroadcast\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/broadcasts/deliveries/{deliveryId}/recipients\n  method: get\n  operationId: listDeliveryRecipients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/broadcasts/deliveries/{deliveryId}/contents/{contentId}/recipients\n\
  \  method: get\n  operationId: listContentRecipients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/ourpeople/refs/heads/main/agentic-access/ourpeople-agentic-access.yml
summary_line: 6 operations · 2 acting
tags:
- Communications
- Workforce
- Frontline
---
