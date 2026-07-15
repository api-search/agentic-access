---
acting_count: 2
action_class_counts:
  acting: 2
  connected: 2
api_specs:
- filename: wati-openapi.yml
  format: yaml
  label: WATI WhatsApp Business API
  slug: whatsapp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wati/refs/heads/main/openapi/wati-openapi.yml
consequence_counts:
  physical: 2
  read: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Wati Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sendSessionMessage/{whatsappNumber}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sendTemplateMessage
operation_count: 4
overview: 'WATI exposes 4 API operations that an AI agent could call, of which 2 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 2 read and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: WATI
provider_slug: wati
slug: wati-agentic-access
source_filename: wati-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/wati-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 4\n  by_action_class:\n    connected: 2\n    acting: 2\n  by_consequence:\n    read: 2\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /getContacts\n  method: get\n  operationId: getContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /getMessages/{whatsappNumber}\n  method: get\n  operationId: getMessagesByNumber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sendTemplateMessage\n\
  \  method: post\n  operationId: sendTemplateMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sendSessionMessage/{whatsappNumber}\n  method: post\n  operationId: sendSessionMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wati/refs/heads/main/agentic-access/wati-agentic-access.yml
summary_line: 4 operations · 2 acting
tags:
- WhatsApp
- Messaging
- Customer Engagement
- Chatbot
- Business Communication
- CRM
---
