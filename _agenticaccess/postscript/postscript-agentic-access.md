---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 11
api_specs:
- filename: postscript-partner-api-openapi.yml
  format: yaml
  label: Postscript Partner API
  slug: postscript-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postscript/refs/heads/main/openapi/_original/postscript-partner-api-openapi.yml
- filename: postscript-subscribers-api-openapi.yml
  format: yaml
  label: Postscript Subscribers API
  slug: postscript-subscribers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postscript/refs/heads/main/openapi/postscript-subscribers-api-openapi.yml
- filename: postscript-events-api-openapi.yml
  format: yaml
  label: Postscript Events API
  slug: postscript-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postscript/refs/heads/main/openapi/postscript-events-api-openapi.yml
- filename: postscript-keywords-api-openapi.yml
  format: yaml
  label: Postscript Keywords API
  slug: postscript-keywords-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postscript/refs/heads/main/openapi/postscript-keywords-api-openapi.yml
- filename: postscript-messages-api-openapi.yml
  format: yaml
  label: Postscript Messages API
  slug: postscript-messages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postscript/refs/heads/main/openapi/postscript-messages-api-openapi.yml
- filename: postscript-webhooks-api-openapi.yml
  format: yaml
  label: Postscript Webhooks API
  slug: postscript-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postscript/refs/heads/main/openapi/postscript-webhooks-api-openapi.yml
- filename: postscript-compliance-api-openapi.yml
  format: yaml
  label: Postscript Compliance API
  slug: postscript-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postscript/refs/heads/main/openapi/postscript-compliance-api-openapi.yml
- filename: postscript-identity-api-openapi.yml
  format: yaml
  label: Postscript Identity API
  slug: postscript-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/postscript/refs/heads/main/openapi/postscript-identity-api-openapi.yml
consequence_counts:
  physical: 1
  read: 11
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Postscript Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/message_requests
operation_count: 20
overview: 'Postscript exposes 20 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 8 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Postscript
provider_slug: postscript
slug: postscript-agentic-access
source_filename: postscript-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-13'\nmethod: generated\nsource: openapi/postscript-compliance-api-openapi.yml, openapi/postscript-events-api-openapi.yml,\n  openapi/postscript-identity-api-openapi.yml, openapi/postscript-keywords-api-openapi.yml,\n  openapi/postscript-messages-api-openapi.yml, openapi/postscript-subscribers-api-openapi.yml,\n  openapi/postscript-webhooks-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 20\n  by_action_class:\n    acting: 9\n    connected: 11\n  by_consequence:\n    write: 8\n    read: 11\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v2/compliance/redact\n  method: patch\n  operationId: redact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/compliance/unsubscribe\n  method: patch\n  operationId: unsubscribe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/events\n  method: post\n  operationId: create-custom-event\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/me\n  method: get\n  operationId: verify-identity\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/keywords\n  method: get\n  operationId: get-keywords\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/keywords/{id}\n  method: get\n  operationId: get-keyword\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/message_requests\n  method: post\n  operationId: create-message\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/message_requests/{id}\n\
  \  method: get\n  operationId: get-message-request\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/sent_messages/{id}\n  method: get\n  operationId: get-sent-message\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/subscribers\n  method: get\n  operationId: get-subscribers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/subscribers/{id}\n  method: get\n  operationId: get-subscriber\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/subscribers/{id}\n  method: patch\n  operationId: update-subscriber-by-id\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/webhooks\n  method: post\n  operationId: create-webhook-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/webhooks\n  method: get\n  operationId: list-webhook-subscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/webhooks/{id}\n  method: delete\n  operationId: delete-webhook-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/webhooks/{id}\n  method: get\n  operationId: get-webhook-subscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/webhooks/{id}\n  method: patch\n  operationId: update-webhook-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/webhooks/example\n  method: get\n  operationId: example-event\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /api/v2/webhooks/test\n  method: post\n  operationId: test-shop-webhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/webhooks/token\n  method: get\n  operationId: get-webhook-signing-token\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/postscript/refs/heads/main/agentic-access/postscript-agentic-access.yml
summary_line: 20 operations · 9 acting
tags:
- SMS
- Marketing
- Messaging
- E-commerce
- Shopify
- RCS
- Subscribers
- Webhooks
- Compliance
---
