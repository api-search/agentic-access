---
acting_count: 6
action_class_counts:
  acting: 6
  connected: 7
api_specs:
- filename: telstra-messaging-api-openapi.yml
  format: yaml
  label: Telstra Messaging API
  slug: telstra-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telstra/refs/heads/main/openapi/telstra-messaging-api-openapi.yml
- filename: telstra-mobile-number-verification-api-openapi.yml
  format: yaml
  label: Telstra Mobile Number Verification API
  slug: telstra-mobile-number-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/telstra/refs/heads/main/openapi/telstra-mobile-number-verification-api-openapi.yml
consequence_counts:
  physical: 4
  read: 7
  write: 2
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Telstra Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /messages/mms
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /messages/provisioning/subscriptions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /messages/provisioning/subscriptions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /messages/sms
operation_count: 13
overview: 'Telstra exposes 13 API operations that an AI agent could call, of which 6 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read, 2 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Telstra
provider_slug: telstra
slug: telstra-agentic-access
source_filename: telstra-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/telstra-messaging-api-openapi.yml, openapi/telstra-mobile-number-verification-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 13\n  by_action_class:\n    acting: 6\n    connected: 7\n  by_consequence:\n    write: 2\n    physical: 4\n    read: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /oauth/token\n  method: post\n  operationId: generateToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - NSMS\n- path: /messages/sms\n\
  \  method: post\n  operationId: sendSms\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - NSMS\n- path: /messages/sms\n  method: get\n  operationId: getSmsReplies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - NSMS\n- path: /messages/sms/{messageId}/status\n  method: get\n  operationId: getSmsStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - NSMS\n- path: /messages/sms/healthcheck\n  method: get\n  operationId: smsHealthcheck\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - NSMS\n- path: /messages/mms\n  method: post\n  operationId: sendMms\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - NSMS\n- path: /messages/mms\n  method: get\n  operationId: getMmsReplies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - NSMS\n- path: /messages/mms/{messageId}/status\n  method: get\n  operationId: getMmsStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n    scope:\n    - NSMS\n- path: /messages/mms/healthcheck\n  method: get\n  operationId: mmsHealthcheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n    - NSMS\n- path: /messages/provisioning/subscriptions\n  method: post\n  operationId: createSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - NSMS\n- path: /messages/provisioning/subscriptions\n  method: get\n  operationId: getSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n    scope:\n  \
  \  - NSMS\n- path: /messages/provisioning/subscriptions\n  method: delete\n  operationId: deleteSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - NSMS\n- path: /mobile-number-verification/verify\n  method: post\n  operationId: verifyMobileNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n    scope:\n    - MNV\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/telstra/refs/heads/main/agentic-access/telstra-agentic-access.yml
summary_line: 13 operations · 6 acting
tags:
- Telecommunications
- Telco
- Mobile
- Messaging
- SMS
- MMS
- Networks
- Australia
- Verification
---
