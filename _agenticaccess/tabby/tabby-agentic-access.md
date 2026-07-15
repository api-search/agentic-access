---
acting_count: 12
action_class_counts:
  acting: 12
  connected: 7
api_specs:
- filename: tabby-api-openapi.yml
  format: yaml
  label: Tabby Checkout API
  slug: tabby-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabby/refs/heads/main/openapi/tabby-api-openapi.yml
- filename: tabby-api-openapi.yml
  format: yaml
  label: Tabby Payments API
  slug: tabby-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabby/refs/heads/main/openapi/tabby-api-openapi.yml
- filename: tabby-api-openapi.yml
  format: yaml
  label: Tabby Webhooks API
  slug: tabby-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabby/refs/heads/main/openapi/tabby-api-openapi.yml
- filename: tabby-api-openapi.yml
  format: yaml
  label: Tabby Disputes API
  slug: tabby-disputes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tabby/refs/heads/main/openapi/tabby-api-openapi.yml
consequence_counts:
  physical: 5
  read: 7
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Tabby Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/v2/payments/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/payments/{id}/captures
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/payments/{id}/close
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/payments/{id}/refunds
operation_count: 19
overview: 'Tabby exposes 19 API operations that an AI agent could call, of which 12 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 7 read, 7 write, and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Tabby
provider_slug: tabby
slug: tabby-agentic-access
source_filename: tabby-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/tabby-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 19\n  by_action_class:\n    acting: 12\n    connected: 7\n  by_consequence:\n    physical: 5\n    read: 7\n    write: 7\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v2/checkout\n  method: post\n  operationId: postCheckoutSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - secret_key\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/checkout/{id}\n\
  \  method: get\n  operationId: getCheckoutSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - secret_key\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/payments/{id}\n  method: get\n  operationId: getPayment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - secret_key\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/payments/{id}\n  method: put\n  operationId: putPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - secret_key\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/payments/{id}/captures\n  method: post\n  operationId: postPaymentCapture\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - secret_key\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/payments/{id}/refunds\n  method: post\n  operationId: postPaymentRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - secret_key\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/payments/{id}/close\n  method: post\n  operationId: closePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n\
  \    - secret_key\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/payments\n  method: get\n  operationId: getPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - secret_key\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhooks\n  method: post\n  operationId: postWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - secret_key\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/webhooks\n  method: get\n  operationId: getWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    scope:\n    - secret_key\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhooks/{id}\n  method: get\n  operationId: getWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - secret_key\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhooks/{id}\n  method: put\n  operationId: putWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - secret_key\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/webhooks/{id}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - secret_key\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/disputes\n  method: get\n  operationId: getDisputes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - secret_key\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/disputes/{disputeId}\n  method: get\n  operationId: getDispute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - secret_key\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/disputes/{disputeId}/provide-evidence\n  method: post\n  operationId: postDisputeProvideEvidence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - secret_key\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n   \
  \   - high-value\n    audit: required\n- path: /api/v1/disputes/approve\n  method: post\n  operationId: postDisputesApprove\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - secret_key\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/disputes/challenge\n  method: post\n  operationId: postDisputesChallenge\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - secret_key\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/disputes/attachments/upload\n  method: post\n  operationId: postUploadAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n \
  \   subject: required\n    scope:\n    - secret_key\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tabby/refs/heads/main/agentic-access/tabby-agentic-access.yml
summary_line: 19 operations · 12 acting
tags:
- BNPL
- Buy Now Pay Later
- Consumer Finance
- E-commerce
- Fintech
- Installments
- MENA
- Payments
- Saudi Arabia
- UAE
---
