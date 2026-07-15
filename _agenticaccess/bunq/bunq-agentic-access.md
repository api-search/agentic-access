---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 17
api_specs:
- filename: bunq-openapi.yml
  format: yaml
  label: bunq Session (Handshake) API
  slug: bunq-session-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bunq/refs/heads/main/openapi/bunq-openapi.yml
- filename: bunq-openapi.yml
  format: yaml
  label: bunq User API
  slug: bunq-user-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bunq/refs/heads/main/openapi/bunq-openapi.yml
- filename: bunq-openapi.yml
  format: yaml
  label: bunq Monetary Account API
  slug: bunq-monetary-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bunq/refs/heads/main/openapi/bunq-openapi.yml
- filename: bunq-openapi.yml
  format: yaml
  label: bunq Payment API
  slug: bunq-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bunq/refs/heads/main/openapi/bunq-openapi.yml
- filename: bunq-openapi.yml
  format: yaml
  label: bunq Request Inquiry API
  slug: bunq-request-inquiry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bunq/refs/heads/main/openapi/bunq-openapi.yml
- filename: bunq-openapi.yml
  format: yaml
  label: bunq Card API
  slug: bunq-card-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bunq/refs/heads/main/openapi/bunq-openapi.yml
- filename: bunq-openapi.yml
  format: yaml
  label: bunq Attachment API
  slug: bunq-attachment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bunq/refs/heads/main/openapi/bunq-openapi.yml
- filename: bunq-openapi.yml
  format: yaml
  label: bunq Customer Statement (Export) API
  slug: bunq-customer-statement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bunq/refs/heads/main/openapi/bunq-openapi.yml
- filename: bunq-openapi.yml
  format: yaml
  label: bunq Notification Filter (Callbacks) API
  slug: bunq-notification-filter-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/bunq/refs/heads/main/openapi/bunq-openapi.yml
consequence_counts:
  physical: 2
  read: 17
  write: 9
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Bunq Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /user/{userID}/monetary-account/{monetaryAccountID}/draft-payment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /user/{userID}/monetary-account/{monetaryAccountID}/payment
operation_count: 28
overview: 'bunq exposes 28 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 17 read, 9 write, and 2 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: bunq
provider_slug: bunq
slug: bunq-agentic-access
source_filename: bunq-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/bunq-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 28\n  by_action_class:\n    acting: 11\n    connected: 17\n  by_consequence:\n    write: 9\n    read: 17\n    physical: 2\n  human_in_the_loop_required: 0\noperations:\n- path: /installation\n  method: post\n  operationId: createInstallation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /device-server\n  method: post\n  operationId: createDeviceServer\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /session-server\n  method: post\n  operationId: createSessionServer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user\n  method: get\n  operationId: listUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/{userID}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /user/{userID}/monetary-account\n  method: get\n  operationId: listMonetaryAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/{userID}/monetary-account/{monetaryAccountID}\n  method: get\n  operationId: getMonetaryAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/{userID}/monetary-account-bank\n  method: get\n  operationId: listMonetaryAccountBank\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/{userID}/monetary-account-bank\n  method: post\n  operationId: createMonetaryAccountBank\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/{userID}/monetary-account/{monetaryAccountID}/payment\n  method: get\n  operationId: listPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/{userID}/monetary-account/{monetaryAccountID}/payment\n  method: post\n  operationId: createPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/{userID}/monetary-account/{monetaryAccountID}/payment/{paymentID}\n  method: get\n  operationId: getPayment\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/{userID}/monetary-account/{monetaryAccountID}/draft-payment\n  method: get\n  operationId: listDraftPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/{userID}/monetary-account/{monetaryAccountID}/draft-payment\n  method: post\n  operationId: createDraftPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/{userID}/monetary-account/{monetaryAccountID}/request-inquiry\n  method: get\n  operationId: listRequestInquiries\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/{userID}/monetary-account/{monetaryAccountID}/request-inquiry\n  method: post\n  operationId: createRequestInquiry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/{userID}/monetary-account/{monetaryAccountID}/request-response\n  method: get\n  operationId: listRequestResponses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/{userID}/card\n  method: get\n  operationId: listCards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/{userID}/card/{cardID}\n\
  \  method: get\n  operationId: getCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/{userID}/attachment-public\n  method: post\n  operationId: createAttachmentPublic\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /attachment-public/{attachmentPublicUUID}/content\n  method: get\n  operationId: getAttachmentPublicContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/{userID}/monetary-account/{monetaryAccountID}/customer-statement\n  method: get\n  operationId: listCustomerStatements\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/{userID}/monetary-account/{monetaryAccountID}/customer-statement\n  method: post\n  operationId: createCustomerStatement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/{userID}/monetary-account/{monetaryAccountID}/customer-statement/{customerStatementID}/content\n  method: get\n  operationId: getCustomerStatementContent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/{userID}/notification-filter-url\n  method: get\n  operationId: listNotificationFilterUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/{userID}/notification-filter-url\n  method: post\n  operationId: createNotificationFilterUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user/{userID}/notification-filter-push\n  method: get\n  operationId: listNotificationFilterPush\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user/{userID}/notification-filter-push\n  method: post\n  operationId: createNotificationFilterPush\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/bunq/refs/heads/main/agentic-access/bunq-agentic-access.yml
summary_line: 28 operations · 11 acting
tags:
- Banking
- Neobank
- Payments
- Accounts
- SEPA
- Open Banking
- Fintech
- Europe
- Netherlands
---
