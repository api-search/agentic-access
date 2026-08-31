---
acting_count: 32
action_class_counts:
  acting: 32
  connected: 3
api_specs:
- filename: till-payments-continue-dcc-api-openapi.yml
  format: yaml
  label: Till Payments Continue Dcc API
  slug: till-payments-continue-dcc-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/till-payments/refs/heads/main/openapi/till-payments-continue-dcc-api-openapi.yml
- filename: till-payments-dispute-api-openapi.yml
  format: yaml
  label: Till Payments Dispute API
  slug: till-payments-dispute-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/till-payments/refs/heads/main/openapi/till-payments-dispute-api-openapi.yml
- filename: till-payments-options-api-openapi.yml
  format: yaml
  label: Till Payments Options API
  slug: till-payments-options-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/till-payments/refs/heads/main/openapi/till-payments-options-api-openapi.yml
- filename: till-payments-prepare-transaction-api-openapi.yml
  format: yaml
  label: Till Payments Prepare Transaction API
  slug: till-payments-prepare-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/till-payments/refs/heads/main/openapi/till-payments-prepare-transaction-api-openapi.yml
- filename: till-payments-schedule-api-openapi.yml
  format: yaml
  label: Till Payments Schedule API
  slug: till-payments-schedule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/till-payments/refs/heads/main/openapi/till-payments-schedule-api-openapi.yml
- filename: till-payments-status-api-openapi.yml
  format: yaml
  label: Till Payments Status API
  slug: till-payments-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/till-payments/refs/heads/main/openapi/till-payments-status-api-openapi.yml
- filename: till-payments-transaction-api-openapi.yml
  format: yaml
  label: Till Payments Transaction API
  slug: till-payments-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/till-payments/refs/heads/main/openapi/till-payments-transaction-api-openapi.yml
consequence_counts:
  physical: 14
  read: 3
  write: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Till Payments Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transaction/{apiKey}/capture
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transaction/{apiKey}/capture
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transaction/{apiKey}/deregister
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transaction/{apiKey}/deregister
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transaction/{apiKey}/incrementalAuthorization
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transaction/{apiKey}/incrementalAuthorization
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transaction/{apiKey}/payout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transaction/{apiKey}/payout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transaction/{apiKey}/preauthorize
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transaction/{apiKey}/preauthorize
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transaction/{apiKey}/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transaction/{apiKey}/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transaction/{apiKey}/register
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transaction/{apiKey}/register
operation_count: 35
overview: 'Till Payments exposes 35 API operations that an AI agent could call, of which 32 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 3 read, 18 write, and 14 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Till Payments
provider_slug: till-payments
slug: till-payments-agentic-access
source_filename: till-payments-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: generated\nsource: openapi/till-payments-direct-pci.yml, openapi/till-payments-gateway.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 35\n  by_action_class:\n    acting: 32\n    connected: 3\n  by_consequence:\n    write: 18\n    physical: 14\n    read: 3\n  human_in_the_loop_required: 0\noperations:\n- path: /transaction/{apiKey}/debit\n  method: post\n  operationId: processDebit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction/{apiKey}/preauthorize\n  method:\
  \ post\n  operationId: processPreauthorize\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction/{apiKey}/incrementalAuthorization\n  method: post\n  operationId: processIncrementalAuthorization\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction/{apiKey}/capture\n  method: post\n  operationId: processCapture\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction/{apiKey}/void\n  method: post\n  operationId: processVoid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction/{apiKey}/register\n  method: post\n  operationId: processRegister\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /transaction/{apiKey}/deregister\n  method: post\n  operationId: processDeregister\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction/{apiKey}/refund\n  method: post\n  operationId: processRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction/{apiKey}/payout\n  method: post\n  operationId: processPayout\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction/{apiKey}/prepare-debit\n  method: post\n  operationId: processPrepareDebit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction/{apiKey}/debit\n  method: post\n  operationId: processDebit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /transaction/{apiKey}/prepare-preauthorize\n  method: post\n  operationId: processPreparePreauthorize\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction/{apiKey}/continue-dcc\n  method: post\n  operationId: processContinueDcc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction/{apiKey}/preauthorize\n  method: post\n  operationId: processPreauthorize\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction/{apiKey}/incrementalAuthorization\n  method: post\n  operationId: processIncrementalAuthorization\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction/{apiKey}/capture\n  method: post\n  operationId: processCapture\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /transaction/{apiKey}/void\n  method: post\n  operationId: processVoid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction/{apiKey}/prepare-register\n  method: post\n  operationId: processPrepareRegister\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction/{apiKey}/register\n  method: post\n  operationId: processRegister\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction/{apiKey}/deregister\n  method: post\n  operationId: processDeregister\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction/{apiKey}/refund\n  method: post\n  operationId: processRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n  \
  \    - abnormal\n      - high-value\n    audit: required\n- path: /transaction/{apiKey}/payout\n  method: post\n  operationId: processPayout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /schedule/{apiKey}/start\n  method: post\n  operationId: startSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /schedule/{apiKey}/{scheduleId}/update\n  method: post\n  operationId: updateSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n  \
  \  subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /schedule/{apiKey}/{scheduleId}/get\n  method: get\n  operationId: getSchedule\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /schedule/{apiKey}/{scheduleId}/pause\n  method: post\n  operationId: pauseSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /schedule/{apiKey}/{scheduleId}/continue\n  method: post\n  operationId: continueSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /schedule/{apiKey}/{scheduleId}/cancel\n  method: post\n  operationId: cancelSchedule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /status/{apiKey}/getByUuid/{uuid}\n  method: get\n  operationId: transactionStatusByUuid\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /status/{apiKey}/getByMerchantTransactionId/{merchantTransactionId}\n  method: get\n  operationId: transactionStatusByMerchantTransactionId\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /options/{apiKey}/{optionsName}\n  method: post\n  operationId: options\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dispute/{apiKey}/accept/{uuid}\n  method: post\n  operationId: accept\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dispute/{apiKey}/metadata/{uuid}\n  method: post\n  operationId: disputeMetadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n  \
  \  audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dispute/{apiKey}/upload-evidence/{uuid}\n  method: post\n  operationId: uploadDisputeEvidence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /dispute/{apiKey}/submit-evidence/{uuid}\n  method: post\n  operationId: submitDisputeEvidence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/till-payments/refs/heads/main/agentic-access/till-payments-agentic-access.yml
summary_line: 35 operations · 32 acting
tags:
- Payments
- Australia
- Payment Gateway
- Payment Processing
- Acquiring
- Merchant Services
- Card Payments
- In-Person Payments
---
