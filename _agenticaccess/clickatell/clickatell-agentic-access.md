---
acting_count: 20
action_class_counts:
  acting: 20
  connected: 9
api_specs:
- filename: clickatell-chat-2-pay-api-api-openapi.yml
  format: yaml
  label: Clickatell Chat 2 Pay API
  slug: clickatell-chat-2-pay-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickatell/refs/heads/main/openapi/clickatell-chat-2-pay-api-api-openapi.yml
- filename: clickatell-chat-2-pay-api-client-callbacks-api-openapi.yml
  format: yaml
  label: Clickatell Chat 2 Pay API Client Callbacks API
  slug: clickatell-chat-2-pay-api-client-callbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickatell/refs/heads/main/openapi/clickatell-chat-2-pay-api-client-callbacks-api-openapi.yml
- filename: clickatell-external-link-callback-api-openapi.yml
  format: yaml
  label: Clickatell External Link Callback API
  slug: clickatell-external-link-callback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickatell/refs/heads/main/openapi/clickatell-external-link-callback-api-openapi.yml
- filename: clickatell-one-api-api-openapi.yml
  format: yaml
  label: Clickatell One API
  slug: clickatell-one-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickatell/refs/heads/main/openapi/clickatell-one-api-api-openapi.yml
- filename: clickatell-one-api-client-callbacks-api-openapi.yml
  format: yaml
  label: Clickatell One API Client Callbacks API
  slug: clickatell-one-api-client-callbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickatell/refs/heads/main/openapi/clickatell-one-api-client-callbacks-api-openapi.yml
- filename: clickatell-sms-api-api-openapi.yml
  format: yaml
  label: Clickatell SMS API
  slug: clickatell-sms-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickatell/refs/heads/main/openapi/clickatell-sms-api-api-openapi.yml
- filename: clickatell-sms-client-callbacks-api-openapi.yml
  format: yaml
  label: Clickatell SMS Client Callbacks API
  slug: clickatell-sms-client-callbacks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickatell/refs/heads/main/openapi/clickatell-sms-client-callbacks-api-openapi.yml
- filename: clickatell-wait-for-callback-api-openapi.yml
  format: yaml
  label: Clickatell Wait for Callback API
  slug: clickatell-wait-for-callback-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/clickatell/refs/heads/main/openapi/clickatell-wait-for-callback-api-openapi.yml
consequence_counts:
  physical: 14
  read: 9
  write: 6
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Clickatell Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/callback/payment-status
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/cancel/{paymentLinkRef}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/chat-2-pay
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/order-receipt
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/payment/{paymentLinkRef}/capture
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/payment/{paymentLinkRef}/reverse
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /client-callback/one-api-reply
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /client-callback/one-api-status
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /client-callback/sms-reply
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /client-callback/sms-status
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /messages/rest/bulk
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/message
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/notification
operation_count: 29
overview: 'Clickatell exposes 29 API operations that an AI agent could call, of which 20 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 9 read, 6 write, and 14 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Clickatell
provider_slug: clickatell
slug: clickatell-agentic-access
source_filename: clickatell-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-13'\nmethod: generated\nsource: openapi/clickatell-chat-2-pay-api-client-callbacks-openapi.json, openapi/clickatell-chat-2-pay-api-openapi.json,\n  openapi/clickatell-flow-openapi.json, openapi/clickatell-one-api-client-callbacks-openapi.json,\n  openapi/clickatell-one-api-openapi.json, openapi/clickatell-sms-api-client-callbacks-openapi.json,\n  openapi/clickatell-sms-api-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 29\n  by_action_class:\n    acting: 20\n    connected: 9\n  by_consequence:\n    write: 6\n    physical: 14\n    read: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v2/callback/transaction-status\n  method: post\n  operationId: testTransactionStatusChangeNotification\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/callback/payment-status\n  method: post\n  operationId: testPaymentStatusChangeNotification\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/callback/config-change\n  method: post\n  operationId: testConfigChangeNotification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/integration\n  method: put\n  operationId: updateIntegrationStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/payment/{paymentLinkRef}/reverse\n  method: post\n  operationId: reverseTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/payment/{paymentLinkRef}/capture\n  method: post\n  operationId: capturePayment\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/chat-2-pay\n  method: post\n  operationId: createPayByLinkTransactionLog\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/order-receipt\n  method: post\n  operationId: createPaymentReceipt\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/cancel/{paymentLinkRef}\n  method: post\n  operationId: cancelLink\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/chat-2-pay/transaction-status\n  method: get\n  operationId: getTransactionStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/config\n  method: get\n  operationId: getConfigSettings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /callback\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /chat/callback\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client-callback/one-api-reply\n  method: post\n  operationId: sendPostOmniReplyCallback\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /client-callback/one-api-status\n  method: post\n  operationId: sendPostOmniStatusCallback\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/message/{omniMessageId}\n  method: get\n  operationId: messageStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/message\n  method: post\n  operationId: sendMessages\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/notification\n  method: post\n  operationId: sendBusinessStatusNotification\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/media/{fileId}\n  method: get\n  operationId: getMetadata\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/media\n  method: get\n  operationId: downloadFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/media\n  method: post\n  operationId:\
  \ uploadFile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/balance\n  method: get\n  operationId: accountMessagingBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client-callback/sms-status\n  method: get\n  operationId: sendGetSmsStatusCallback\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client-callback/sms-status\n  method: post\n  operationId: sendPostSmsStatusCallback\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n   \
  \   exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client-callback/sms-reply\n  method: get\n  operationId: sendGetSmsReplyCallback\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client-callback/sms-reply\n  method: post\n  operationId: sendPostSmsReplyCallback\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages\n  method: post\n  operationId: sendMessageREST_1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages/rest/bulk\n  method: post\n  operationId: sendBulkMessageREST\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /messages/http/send\n  method: get\n  operationId: sendMessageHTTP\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/clickatell/refs/heads/main/agentic-access/clickatell-agentic-access.yml
summary_line: 29 operations · 20 acting
tags:
- Company
- SMS
- WhatsApp
- Messaging
- CPaaS
- Chat Commerce
- Payments
---
