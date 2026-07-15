---
acting_count: 4
action_class_counts:
  acting: 4
  connected: 2
api_specs:
- filename: gupshup-openapi.yml
  format: yaml
  label: Gupshup WhatsApp Messaging API
  slug: gupshup-whatsapp-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gupshup/refs/heads/main/openapi/gupshup-openapi.yml
- filename: gupshup-openapi.yml
  format: yaml
  label: Gupshup WhatsApp Template Messaging API
  slug: gupshup-whatsapp-template-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gupshup/refs/heads/main/openapi/gupshup-openapi.yml
- filename: gupshup-openapi.yml
  format: yaml
  label: Gupshup WhatsApp Opt-In Management API
  slug: gupshup-whatsapp-optin-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/gupshup/refs/heads/main/openapi/gupshup-openapi.yml
consequence_counts:
  physical: 2
  read: 2
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Gupshup Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /msg
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /template/msg
operation_count: 6
overview: 'Gupshup exposes 6 API operations that an AI agent could call, of which 4 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read, 2 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Gupshup
provider_slug: gupshup
slug: gupshup-agentic-access
source_filename: gupshup-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/gupshup-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 6\n  by_action_class:\n    acting: 4\n    connected: 2\n  by_consequence:\n    physical: 2\n    read: 2\n    write: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /msg\n  method: post\n  operationId: sendMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /template/msg\n  method: post\n  operationId: sendTemplateMessage\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /template/list/{appName}\n  method: get\n  operationId: listTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /app/opt/in/{appName}\n  method: post\n  operationId: markUserOptIn\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /app/opt/out/{appName}\n  method: post\n  operationId: markUserOptOut\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{appName}\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/gupshup/refs/heads/main/agentic-access/gupshup-agentic-access.yml
summary_line: 6 operations · 4 acting
tags:
- Messaging
- WhatsApp
- Conversational AI
- CPaaS
- SMS
- RCS
- India
- Chatbots
- Business Messaging
- Communications
---
