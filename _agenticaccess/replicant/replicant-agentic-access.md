---
acting_count: 2
action_class_counts:
  acting: 2
api_specs:
- filename: replicant-replicant-api-openapi.yml
  format: yaml
  label: Replicant Replicant API
  slug: replicant-replicant-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/replicant/refs/heads/main/openapi/replicant-replicant-api-openapi.yml
consequence_counts:
  physical: 1
  write: 1
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Replicant Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /campaigns/{campaignId}/sms
operation_count: 2
overview: 'Replicant exposes 2 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 1 write and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Replicant
provider_slug: replicant
slug: replicant-agentic-access
source_filename: replicant-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-14'\nmethod: generated\nsource: openapi/replicant-outbound-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 2\n  by_action_class:\n    acting: 2\n  by_consequence:\n    write: 1\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /campaigns/{campaignId}/calls\n  method: post\n  operationId: placeCall\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /campaigns/{campaignId}/sms\n  method: post\n  operationId: sendSMS\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/replicant/refs/heads/main/agentic-access/replicant-agentic-access.yml
summary_line: 2 operations · 2 acting
tags:
- Company
- Contact Center
- Conversational AI
- Customer Service
- Voice AI
- Contact Center Automation
- Agentic AI
- Conversation Intelligence
---
