---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 11
api_specs:
- filename: engagespark-openapi-original.yml
  format: yaml
  label: engageSPARK API
  slug: engagespark-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/engagespark/refs/heads/main/openapi/engagespark-openapi-original.yml
consequence_counts:
  physical: 4
  read: 11
  write: 8
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Engagespark Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/organizations/{orgId}/topup/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/sms/contact
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/sms/phonenumber
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/whatsapp/contact
operation_count: 23
overview: 'engageSPARK exposes 23 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 11 read, 8 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: engageSPARK
provider_slug: engagespark
slug: engagespark-agentic-access
source_filename: engagespark-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/engagespark-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    connected: 11\n    acting: 12\n  by_consequence:\n    read: 11\n    write: 8\n    physical: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/organizations/{orgId}/balance.json\n  method: get\n  operationId: getOrgBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations/{orgId}/engagements/{campaignId}/subscribe\n  method: post\n  operationId: subscribeContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/organizations/{orgId}/engagements/{campaignId}/unsubscribe\n  method: post\n  operationId: unsubscribeContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/organizations/{orgId}/contacts/\n  method: get\n  operationId: listContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations/{orgId}/contacts/\n  method: post\n  operationId: createContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/organizations/{orgId}/contacts/{contactId}/\n  method: get\n  operationId: getContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations/{orgId}/contacts/{contactId}/\n  method: put\n  operationId: updateContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/organizations/{orgId}/contacts/{contactId}/\n  method: delete\n  operationId: deleteContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sms/contact\n  method: post\n  operationId: sendSmsContact\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/sms/phonenumber\n  method: post\n  operationId: sendSmsPhonenumber\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v1/organizations/{orgId}/messages/\n  method: get\n  operationId: getSmsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations/{orgId}/messages/{messageId}/\n  method: get\n  operationId: getSms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations/{orgId}/files/\n  method: get\n  operationId: getFileList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations/{orgId}/files/\n  method: post\n  operationId: uploadFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/organizations/{orgId}/files/{filename}\n  method: get\n  operationId: downloadFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations/{orgId}/files/{filename}\n  method: post\n  operationId: updateFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/organizations/{orgId}/files/{filename}\n  method: delete\n  operationId: deleteFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/organizations/{orgId}/topup/\n  method: post\n  operationId: sendOrgTopup\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/organizations/{orgId}/topups/\n  method: get\n  operationId: getOrgTopupsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations/{orgId}/topups/{topupId}/\n  method: get\n  operationId: getOrgTopups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/whatsapp/contact\n  method: post\n\
  \  operationId: sendWhatsAppContact\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/organizations/{orgId}/whatsapp/\n  method: get\n  operationId: getWhatsAppList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/organizations/{orgId}/whatsapp/{messageId}/\n  method: get\n  operationId: getWhatsApp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/engagespark/refs/heads/main/agentic-access/engagespark-agentic-access.yml
summary_line: 23 operations · 12 acting
tags:
- Company
- Messaging
- SMS
- Voice
- WhatsApp
- Airtime
- Communications
- CPaaS
- Surveys
- International Development
---
