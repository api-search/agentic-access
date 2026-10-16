---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 8
api_specs:
- filename: bulksms-attachments-api-openapi.yml
  format: yaml
  label: BulkSMS Attachments API
  slug: bulksms-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bulksms/refs/heads/main/openapi/bulksms-attachments-api-openapi.yml
- filename: bulksms-blocked-numbers-api-openapi.yml
  format: yaml
  label: BulkSMS Blocked Numbers API
  slug: bulksms-blocked-numbers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bulksms/refs/heads/main/openapi/bulksms-blocked-numbers-api-openapi.yml
- filename: bulksms-credits-api-openapi.yml
  format: yaml
  label: BulkSMS Credits API
  slug: bulksms-credits-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bulksms/refs/heads/main/openapi/bulksms-credits-api-openapi.yml
- filename: bulksms-message-api-openapi.yml
  format: yaml
  label: BulkSMS Message API
  slug: bulksms-message-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bulksms/refs/heads/main/openapi/bulksms-message-api-openapi.yml
- filename: bulksms-profile-api-openapi.yml
  format: yaml
  label: BulkSMS Profile API
  slug: bulksms-profile-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bulksms/refs/heads/main/openapi/bulksms-profile-api-openapi.yml
- filename: bulksms-webhooks-api-openapi.yml
  format: yaml
  label: BulkSMS Webhooks API
  slug: bulksms-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bulksms/refs/heads/main/openapi/bulksms-webhooks-api-openapi.yml
consequence_counts:
  physical: 2
  read: 8
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bulksms Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /credit/transfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /messages
operation_count: 15
overview: 'BulkSMS exposes 15 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 5 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: BulkSMS
provider_slug: bulksms
slug: bulksms-agentic-access
source_filename: bulksms-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/bulksms-openapi.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 15\n  by_action_class:\n    connected: 8\n    acting: 7\n  by_consequence:\n    read: 8\n    physical: 2\n    write: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /messages\n  method: get\n  operationId: message.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /messages\n  method: post\n  operationId: message.send\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages/{id}\n  method: get\n  operationId: message.show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /messages/{id}/relatedReceivedMessages\n  method: get\n  operationId: message.related.received\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /messages/send\n  method: get\n  operationId: message.send.simple.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /profile\n  method: get\n  operationId: profile.show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n \
  \     max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: get\n  operationId: webhook.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: post\n  operationId: webhook.create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{id}\n  method: get\n  operationId: webhook.show\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{id}\n  method: post\n  operationId: webhook.update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{id}\n  method: delete\n  operationId: webhook.delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /blocked-numbers\n  method: get\n  operationId: blocked.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /blocked-numbers\n  method: post\n  operationId: blocked.create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /credit/transfer\n  method: post\n  operationId: credit.transfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rmm/pre-sign-attachment\n  method: post\n  operationId: attachment.presign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bulksms/refs/heads/main/agentic-access/bulksms-agentic-access.yml
summary_line: 15 operations · 7 acting
tags:
- SMS
- Messaging
- Communications
- Business
- BulkSMS
---
