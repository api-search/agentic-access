---
acting_count: 22
action_class_counts:
  acting: 22
  connected: 20
api_specs:
- filename: clicksend-openapi.yml
  format: yaml
  label: ClickSend SMS API
  slug: clicksend-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-openapi.yml
- filename: clicksend-openapi.yml
  format: yaml
  label: ClickSend MMS API
  slug: clicksend-mms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-openapi.yml
- filename: clicksend-openapi.yml
  format: yaml
  label: ClickSend Voice / Text-to-Speech API
  slug: clicksend-voice-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-openapi.yml
- filename: clicksend-openapi.yml
  format: yaml
  label: ClickSend Transactional Email API
  slug: clicksend-email-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-openapi.yml
- filename: clicksend-openapi.yml
  format: yaml
  label: ClickSend Post - Letters API
  slug: clicksend-post-letters-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-openapi.yml
- filename: clicksend-openapi.yml
  format: yaml
  label: ClickSend Post - Postcards API
  slug: clicksend-post-postcards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-openapi.yml
- filename: clicksend-openapi.yml
  format: yaml
  label: ClickSend Contacts & Lists API
  slug: clicksend-contacts-lists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-openapi.yml
- filename: clicksend-openapi.yml
  format: yaml
  label: ClickSend Delivery Receipts & Inbound API
  slug: clicksend-delivery-receipts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-openapi.yml
- filename: clicksend-openapi.yml
  format: yaml
  label: ClickSend Account & Balance API
  slug: clicksend-account-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/openapi/clicksend-openapi.yml
consequence_counts:
  physical: 12
  read: 20
  write: 10
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Clicksend Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /email/price
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /email/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /mms/price
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /mms/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /post/letters/price
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /post/letters/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /post/postcards/price
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /post/postcards/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sms/price
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sms/send
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /voice/price
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /voice/send
operation_count: 42
overview: 'ClickSend exposes 42 API operations that an AI agent could call, of which 22 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read, 10 write, and 12 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: ClickSend
provider_slug: clicksend
slug: clicksend-agentic-access
source_filename: clicksend-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/clicksend-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 42\n  by_action_class:\n    acting: 22\n    connected: 20\n  by_consequence:\n    physical: 12\n    read: 20\n    write: 10\n  human_in_the_loop_required: 0\noperations:\n- path: /sms/send\n  method: post\n  operationId: smsSendPost\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sms/price\n  method: post\n  operationId: smsPricePost\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sms/history\n  method: get\n  operationId: smsHistoryGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sms/{message_id}/cancel\n  method: put\n  operationId: smsCancelPut\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sms/templates\n  method: get\n  operationId: smsTemplatesGet\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mms/send\n  method: post\n  operationId: mmsSendPost\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mms/price\n  method: post\n  operationId: mmsPricePost\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mms/history\n  method: get\n  operationId: mmsHistoryGet\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /voice/send\n  method: post\n  operationId: voiceSendPost\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /voice/price\n  method: post\n  operationId: voicePricePost\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /voice/lang\n  method: get\n  operationId: voiceLangGet\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /voice/{message_id}/cancel\n  method: put\n  operationId: voiceCancelPut\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /email/send\n  method: post\n  operationId: emailSendPost\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /email/price\n  method: post\n  operationId: emailPricePost\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /email/history\n  method: get\n  operationId: emailHistoryGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /email/addresses\n  method: get\n  operationId: emailAddressesGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /post/letters/send\n  method: post\n  operationId: postLettersSendPost\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /post/letters/price\n  method: post\n  operationId: postLettersPricePost\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /post/letters/history\n  method: get\n  operationId: postLettersHistoryGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /post/letters/detect-address\n  method: post\n  operationId: postLettersDetectAddressPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /post/postcards/send\n  method: post\n  operationId: postPostcardsSendPost\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /post/postcards/price\n  method: post\n  operationId: postPostcardsPricePost\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /post/postcards/history\n\
  \  method: get\n  operationId: postPostcardsHistoryGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /uploads\n  method: post\n  operationId: uploadsPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lists\n  method: get\n  operationId: listsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lists\n  method: post\n  operationId: listsPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lists/{list_id}/contacts\n  method: get\n  operationId: listContactsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lists/{list_id}/contacts\n  method: post\n  operationId: listContactsPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lists/{list_id}/import\n  method: post\n  operationId: listImportPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /search/contacts-lists\n  method: get\n  operationId: searchContactsLists\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sms/receipts\n  method: get\n  operationId: smsReceiptsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sms/receipts-read\n  method: put\n  operationId: smsReceiptsReadPut\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sms/inbound\n  method: get\n  operationId: smsInboundGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /voice/receipts\n  method: get\n  operationId: voiceReceiptsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mms/receipts\n  method: get\n  operationId: mmsReceiptsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /automations/sms/receipts\n  method: get\n  operationId: automationsSmsReceiptsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /automations/sms/receipts\n  method: post\n  operationId: automationsSmsReceiptsPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /automations/sms/inbound\n  method: get\n  operationId: automationsSmsInboundGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /automations/sms/inbound\n  method: post\n  operationId: automationsSmsInboundPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account\n  method: get\n  operationId: accountGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /account/usage/{year}/{month}/subaccount\n  method: get\n  operationId: accountUsageBySubaccountGet\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subaccounts\n  method: get\n  operationId: subaccountsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clicksend/refs/heads/main/agentic-access/clicksend-agentic-access.yml
summary_line: 42 operations · 22 acting
tags:
- Communications
- SMS
- MMS
- Voice
- Email
- Post
- Messaging
- CPaaS
---
