---
acting_count: 5
action_class_counts:
  acting: 5
  connected: 4
api_specs:
- filename: regal-events-api-openapi.yml
  format: yaml
  label: Regal Events API
  slug: regal-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regal-ai/refs/heads/main/openapi/regal-events-api-openapi.yml
- filename: regal-branded-phone-numbers-api-openapi.yml
  format: yaml
  label: Regal Branded Phone Numbers API
  slug: regal-branded-phone-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regal-ai/refs/heads/main/openapi/regal-branded-phone-numbers-api-openapi.yml
- filename: regal-management-api-openapi.yml
  format: yaml
  label: Regal Management API
  slug: regal-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regal-ai/refs/heads/main/openapi/regal-management-api-openapi.yml
- filename: regal-messages-api-openapi.yml
  format: yaml
  label: Regal Messages API
  slug: regal-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/regal-ai/refs/heads/main/openapi/regal-messages-api-openapi.yml
- filename: regal-reporting-webhooks-asyncapi.yml
  format: yaml
  label: Regal Reporting Webhooks
  slug: regal-reporting-webhooks
  spec_type: AsyncAPI
  url: https://raw.githubusercontent.com/api-evangelist/regal-ai/refs/heads/main/asyncapi/regal-reporting-webhooks-asyncapi.yml
consequence_counts:
  physical: 1
  read: 4
  write: 4
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Regal Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /messages/send
operation_count: 9
overview: 'Regal exposes 9 API operations that an AI agent could call, of which 5 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 4 read, 4 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Regal
provider_slug: regal-ai
slug: regal-ai-agentic-access
source_filename: regal-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/regal-branded-phone-numbers-api-openapi.yml, openapi/regal-events-api-openapi.yml,\n  openapi/regal-management-api-openapi.yml, openapi/regal-messages-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 9\n  by_action_class:\n    acting: 5\n    connected: 4\n  by_consequence:\n    write: 4\n    read: 4\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /brandedPhoneNumbers\n  method: post\n  operationId: postBrandedPhoneNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /brandedPhoneNumbers/{phoneNumber}\n  method: patch\n  operationId: patchBrandedPhoneNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /brandedPhoneNumbers/{phoneNumber}\n  method: delete\n  operationId: deleteBrandedPhoneNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events\n  method: post\n  operationId: postCustomEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /businessProfiles\n  method: get\n  operationId: listBusinessProfiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /activePhoneNumbers\n  method: get\n  operationId: listActivePhoneNumbers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /campaigns\n  method: get\n  operationId: listCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /dispositions\n  method: get\n  operationId: listDispositions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /messages/send\n  method: post\n  operationId: sendMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/regal-ai/refs/heads/main/agentic-access/regal-ai-agentic-access.yml
summary_line: 9 operations · 5 acting
tags:
- AI
- AI Agents
- Voice AI
- Contact Center
- Outbound Calling
- Inbound Calling
- Phone Agents
- SMS
- Chat
- WebRTC
- Conversation Intelligence
- Journey Orchestration
- Branded Caller ID
- CCaaS
- CPaaS
- Sales Dialer
- Customer Engagement
---
