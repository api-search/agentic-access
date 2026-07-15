---
acting_count: 14
action_class_counts:
  acting: 14
  connected: 12
api_specs:
- filename: at-and-t-sms-api.yaml
  format: yaml
  label: AT&T SMS API
  slug: att-sms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/openapi/at-and-t-sms-api.yaml
- filename: at-and-t-in-app-messaging-api.yaml
  format: yaml
  label: AT&T In-App Messaging API
  slug: att-in-app-messaging-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/openapi/at-and-t-in-app-messaging-api.yaml
- filename: at-and-t-mvnx-api.yaml
  format: yaml
  label: AT&T MVNX API
  slug: att-mvnx-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/openapi/at-and-t-mvnx-api.yaml
consequence_counts:
  physical: 6
  read: 12
  safety-critical: 1
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: At And T Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /resource/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /cancelPortabilityOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /myMessages/v2/messages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /portabilityOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /portabilityOrder/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /productOrder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sms/v3/messaging/outbox
operation_count: 26
overview: 'AT&T exposes 26 API operations that an AI agent could call, of which 14 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read, 7 write, 6 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: AT&T
provider_slug: at-and-t
slug: at-and-t-agentic-access
source_filename: at-and-t-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/at-and-t-in-app-messaging-api.yaml, openapi/at-and-t-mvnx-api.yaml, openapi/at-and-t-sms-api.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 26\n  by_action_class:\n    acting: 14\n    connected: 12\n  by_consequence:\n    physical: 6\n    read: 12\n    write: 7\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /myMessages/v2/messages\n  method: post\n  operationId: sendMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - IMMN\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /myMessages/v2/messages\n  method: get\n  operationId: listMessages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - MIM\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /myMessages/v2/messages/{messageId}\n  method: get\n  operationId: getMessage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - MIM\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /myMessages/v2/messages/{messageId}\n  method: put\n  operationId: updateMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - MIM\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /myMessages/v2/messages/{messageId}\n\
  \  method: delete\n  operationId: deleteMessage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - MIM\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /myMessages/v2/messages/index\n  method: post\n  operationId: createMessageIndex\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - MIM\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /myMessages/v2/delta\n  method: get\n  operationId: getInboxDelta\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - MIM\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /geographicSite\n\
  \  method: get\n  operationId: listGeographicSites\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /productOrder\n  method: post\n  operationId: createProductOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /resourceReservation\n  method: post\n  operationId: reserveSubscriberNumber\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /resourceReservation/{id}\n\
  \  method: patch\n  operationId: releaseNumberReservation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portabilityOrder\n  method: post\n  operationId: createPortabilityOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /portabilityOrder\n  method: get\n  operationId: listPortabilityOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portabilityOrder/{id}\n\
  \  method: get\n  operationId: getPortabilityOrder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /portabilityOrder/{id}\n  method: patch\n  operationId: updatePortabilityOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cancelPortabilityOrder\n  method: post\n  operationId: cancelPortabilityOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n  \
  \    - high-value\n    audit: required\n- path: /resource\n  method: get\n  operationId: listResources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/{id}\n  method: get\n  operationId: getResource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /resource/{id}\n  method: patch\n  operationId: updateResource\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /product/{id}\n  method: get\n  operationId: getSubscriberProfile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /service/{id}\n  method: get\n  operationId: getService\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /topupBalance\n  method: post\n  operationId: topupBalance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth/v4/token\n  method: post\n  operationId: getAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sms/v3/messaging/outbox\n\
  \  method: post\n  operationId: sendSms\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - SMS\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sms/v3/messaging/outbox/{messageId}\n  method: get\n  operationId: getSmsDeliveryStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - SMS\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /sms/v3/messaging/inbox/{registrationId}\n  method: get\n  operationId: getInboundSms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - SMS\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/at-and-t/refs/heads/main/agentic-access/at-and-t-agentic-access.yml
summary_line: 26 operations · 14 acting · 1 human-in-the-loop
tags:
- Fortune 100
- Telecommunications
- Wireless
- Wireline
- Messaging
- Speech
- Mobile
- Broadband
- Enterprise
---
