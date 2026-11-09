---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 14
api_specs:
- filename: wbiztool-com-account-api-openapi.yml
  format: yaml
  label: wbiztool-com Account API
  slug: wbiztool-com-account-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wbiztool-com/openapi/wbiztool-com-account-api-openapi.yml
- filename: wbiztool-com-media-api-openapi.yml
  format: yaml
  label: wbiztool-com Media API
  slug: wbiztool-com-media-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wbiztool-com/openapi/wbiztool-com-media-api-openapi.yml
- filename: wbiztool-com-messages-api-openapi.yml
  format: yaml
  label: wbiztool-com Messages API
  slug: wbiztool-com-messages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wbiztool-com/openapi/wbiztool-com-messages-api-openapi.yml
- filename: wbiztool-com-number-verification-api-openapi.yml
  format: yaml
  label: wbiztool-com Number verification API
  slug: wbiztool-com-number-verification-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wbiztool-com/openapi/wbiztool-com-number-verification-api-openapi.yml
- filename: wbiztool-com-reminders-api-openapi.yml
  format: yaml
  label: wbiztool-com Reminders API
  slug: wbiztool-com-reminders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wbiztool-com/openapi/wbiztool-com-reminders-api-openapi.yml
- filename: wbiztool-com-whatsapp-numbers-api-openapi.yml
  format: yaml
  label: wbiztool-com WhatsApp numbers API
  slug: wbiztool-com-whatsapp-numbers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/wbiztool-com/openapi/wbiztool-com-whatsapp-numbers-api-openapi.yml
consequence_counts:
  physical: 3
  read: 14
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Wbiztool Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /send_msg/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /send_msg/group/
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /send_msg/multi/
operation_count: 26
overview: 'wbiztool-com exposes 26 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read, 9 write, and 3 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: wbiztool-com
provider_slug: wbiztool-com
slug: wbiztool-com-agentic-access
source_filename: wbiztool-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-31'\nmethod: generated\nsource: openapi/wbiztool-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 26\n  by_action_class:\n    acting: 12\n    connected: 14\n  by_consequence:\n    physical: 3\n    write: 9\n    read: 14\n  human_in_the_loop_required: 0\noperations:\n- path: /send_msg/\n  method: post\n  operationId: sendMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /send_msg/group/\n  method: post\n  operationId:\
  \ sendGroupMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /send_msg/multi/\n  method: post\n  operationId: sendMultiMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /schedule_msg/\n  method: post\n  operationId: scheduleMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n     \
  \ human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cancel_msg/\n  method: post\n  operationId: cancelMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /message/status/{msg_id}/\n  method: post\n  operationId: getMessageStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /msg_status/\n  method: post\n  operationId: getMessageStatusDeprecated\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /report/\n  method: post\n  operationId: getMessageHistory\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /media/upload/\n  method: post\n  operationId: uploadMedia\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /media/list/\n  method: get\n  operationId: listMedia\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /media/list/\n  method: post\n  operationId: listMediaPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /media/{media_id}/\n  method: get\n  operationId: getMedia\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /media/{media_id}/\n  method: post\n  operationId: getMediaPost\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reminder/create/\n  method: post\n  operationId: createReminder\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /reminder/list/\n  method: post\n  operationId: listReminders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /reminder/cancel/\n  method: post\n  operationId: cancelReminder\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verification/create/\n  method: post\n  operationId: createVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /verification/status/\n  method: get\n  operationId: getVerificationStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /verification/results/\n  method: get\n  operationId: getVerificationResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /whatsapp/connect/\n  method: post\n  operationId: connectWhatsapp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /whatsapp-client/create/\n  method: post\n  operationId: connectWhatsappAlias\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /whatsapp-client/list/\n  method: post\n  operationId: listConnectedNumbers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /whatsapp-client/status/\n  method: post\n  operationId: getConnectionStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /whatsapp/accounts/\n  method: post\n  operationId: listWhatsappAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /me/\n  method: post\n  operationId: checkCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /status/\n  method: get\n  operationId: getApiStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n"
source_yaml_url: https://artifacts.apis.io/wbiztool-com/agentic-access/wbiztool-com-agentic-access.yml
summary_line: 26 operations · 12 acting
tags:
- Company
- WhatsApp
- Messaging
- Automation
- Business
---
