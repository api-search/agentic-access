---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 8
api_specs:
- filename: termii-openapi.yml
  format: yaml
  label: Termii Messaging API
  slug: messaging
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/termii/refs/heads/main/openapi/termii-openapi.yml
- filename: termii-openapi.yml
  format: yaml
  label: Termii Token / OTP API
  slug: token
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/termii/refs/heads/main/openapi/termii-openapi.yml
- filename: termii-openapi.yml
  format: yaml
  label: Termii Sender IDs API
  slug: sender-ids
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/termii/refs/heads/main/openapi/termii-openapi.yml
- filename: termii-openapi.yml
  format: yaml
  label: Termii Campaigns API
  slug: campaigns
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/termii/refs/heads/main/openapi/termii-openapi.yml
- filename: termii-openapi.yml
  format: yaml
  label: Termii Contacts / Phonebooks API
  slug: contacts
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/termii/refs/heads/main/openapi/termii-openapi.yml
- filename: termii-openapi.yml
  format: yaml
  label: Termii Insights API
  slug: insights
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/termii/refs/heads/main/openapi/termii-openapi.yml
consequence_counts:
  physical: 7
  read: 8
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Termii Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sender-id/request
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sms/campaigns/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sms/number/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sms/otp/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sms/otp/send/voice
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sms/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sms/send/bulk
operation_count: 24
overview: 'Termii exposes 24 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read, 9 write, and 7 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Termii
provider_slug: termii
slug: termii-agentic-access
source_filename: termii-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/termii-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 24\n  by_action_class:\n    acting: 16\n    connected: 8\n  by_consequence:\n    physical: 7\n    write: 9\n    read: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /sms/send\n  method: post\n  operationId: sendMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sms/send/bulk\n  method: post\n  operationId: sendBulkMessage\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sms/number/send\n  method: post\n  operationId: sendViaNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sms/otp/send\n  method: post\n  operationId: sendToken\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sms/otp/send/voice\n  method: post\n  operationId: sendVoiceToken\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sms/otp/generate\n  method: post\n  operationId: generateInAppToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sms/otp/verify\n  method: post\n  operationId: verifyToken\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sender-id\n  method: get\n  operationId: fetchSenderIds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sender-id/request\n  method: post\n  operationId: requestSenderId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sms/campaigns/send\n  method: post\n  operationId: sendCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sms/campaigns\n  method: get\n  operationId: fetchCampaigns\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sms/campaigns/{campaign_id}\n  method: get\n  operationId: fetchCampaignHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sms/campaigns/{campaign_id}\n  method: patch\n  operationId: retryCampaign\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /phonebooks\n  method: get\n  operationId: listPhonebooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /phonebooks\n  method: post\n  operationId: createPhonebook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /phonebooks/{phonebook_id}\n  method: patch\n  operationId: updatePhonebook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /phonebooks/{phonebook_id}\n  method: delete\n  operationId: deletePhonebook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /phonebooks/{phonebook_id}/contacts\n  method: get\n  operationId: listContacts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /phonebooks/{phonebook_id}/contacts\n  method: post\n  operationId: addContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /phonebooks/{phonebook_id}/contacts\n\
  \  method: delete\n  operationId: deleteContact\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /phonebooks/contacts/upload\n  method: post\n  operationId: uploadContacts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /get-balance\n  method: get\n  operationId: getBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sms/inbox\n  method: get\n  operationId: getMessageHistory\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insight/number/query\n  method: get\n  operationId: queryNumberStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/termii/refs/heads/main/agentic-access/termii-agentic-access.yml
summary_line: 24 operations · 16 acting
tags:
- Messaging
- SMS
- OTP
- WhatsApp
- Verification
---
