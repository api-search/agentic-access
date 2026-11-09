---
acting_count: 9
action_class_counts:
  acting: 9
  connected: 10
api_specs:
- filename: blinkinbox-club-account-api-openapi.yml
  format: yaml
  label: blinkinbox-club Account API
  slug: blinkinbox-club-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blinkinbox-club/openapi/blinkinbox-club-account-api-openapi.yml
- filename: blinkinbox-club-domains-api-openapi.yml
  format: yaml
  label: blinkinbox-club Domains API
  slug: blinkinbox-club-domains-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blinkinbox-club/openapi/blinkinbox-club-domains-api-openapi.yml
- filename: blinkinbox-club-inboxes-api-openapi.yml
  format: yaml
  label: blinkinbox-club Inboxes API
  slug: blinkinbox-club-inboxes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blinkinbox-club/openapi/blinkinbox-club-inboxes-api-openapi.yml
- filename: blinkinbox-club-messages-api-openapi.yml
  format: yaml
  label: blinkinbox-club Messages API
  slug: blinkinbox-club-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blinkinbox-club/openapi/blinkinbox-club-messages-api-openapi.yml
- filename: blinkinbox-club-webhooks-api-openapi.yml
  format: yaml
  label: blinkinbox-club Webhooks API
  slug: blinkinbox-club-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/blinkinbox-club/openapi/blinkinbox-club-webhooks-api-openapi.yml
consequence_counts:
  physical: 1
  read: 10
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Blinkinbox Club Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /webhooks/{id}/test
operation_count: 19
overview: 'blinkinbox-club exposes 19 API operations that an AI agent could call, of which 9 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 10 read, 8 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: blinkinbox-club
provider_slug: blinkinbox-club
slug: blinkinbox-club-agentic-access
source_filename: blinkinbox-club-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/blinkinbox-club-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    acting: 9\n    connected: 10\n  by_consequence:\n    write: 8\n    read: 10\n    physical: 1\n  human_in_the_loop_required: 0\noperations:\n- path: /inboxes\n  method: post\n  operationId: createInbox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inboxes\n  method: get\n  operationId: listInboxes\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inboxes/{inbox}\n  method: get\n  operationId: getInbox\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inboxes/{inbox}\n  method: delete\n  operationId: deleteInbox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inboxes/{inbox}/messages\n  method: get\n  operationId: listMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inboxes/{inbox}/messages/wait\n  method: get\n  operationId: waitForMessage\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inboxes/{inbox}/otp\n  method: get\n  operationId: getLatestOtp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inboxes/{inbox}/messages/{id}\n  method: get\n  operationId: getMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /inboxes/{inbox}/messages/{id}\n  method: delete\n  operationId: deleteMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /inboxes/{inbox}/messages/{id}/attachments/{attachmentId}\n  method: get\n\
  \  operationId: downloadAttachment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domains\n  method: get\n  operationId: listDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /domains\n  method: post\n  operationId: addDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domains/{id}/verify\n  method: post\n  operationId: verifyDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /domains/{id}\n  method: delete\n  operationId: deleteDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: createWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{id}\n\
  \  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{id}/test\n  method: post\n  operationId: testWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /me\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/blinkinbox-club/agentic-access/blinkinbox-club-agentic-access.yml
summary_line: 19 operations · 9 acting
tags:
- Email
- MCP
- Developer Tools
- Disposable
---
