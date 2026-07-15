---
acting_count: 128
action_class_counts:
  acting: 128
  connected: 70
api_specs:
- filename: openapi
  format: yaml
  label: Root Platform API
  slug: root-platform-api
  spec_type: OpenAPI
  url: https://api.rootplatform.com/v1/docs/insurance/openapi
consequence_counts:
  physical: 27
  read: 70
  safety-critical: 1
  write: 100
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Root Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /webhooks/{webhook_id}/disable
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /applications/{application_id}/payment-method
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /applications/{application_id}/send-application-pdf-to-policyholder
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /claims/fulfillment-requests/{fulfillment_request_id}/approve
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /claims/fulfillment-requests/{fulfillment_request_id}/reject
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /claims/{claim_id}/send-to-capture
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /claims/{claim_id}/send-to-review
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /payment-batches/{payment_batch_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment-methods/debicheck-mandates
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /payment-methods/debicheck-mandates/{mandate_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment-methods/{payment_method_id}/dismiss
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment-methods/{payment_method_id}/manual-verify
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /payment-methods/{payment_method_id}/verification-status
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/async-create
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/async-update
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /payments/{payment_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /payout-requests/{payout_request_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /policies/{policy_id}/payment-coupons
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /policies/{policy_id}/payment-coupons
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /policies/{policy_id}/payment-coupons/{payment_coupon_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /policies/{policy_id}/payment-coupons/{payment_coupon_id}/redeem
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /policies/{policy_id}/payment-method
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /policies/{policy_id}/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /policies/{policy_id}/payments/allocate-eft
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /policies/{policy_id}/payments/request-collection
operation_count: 198
overview: 'Root Insurance exposes 198 API operations that an AI agent could call, of which 128 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 70 read, 100 write, 27 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Root Insurance
provider_slug: root
slug: root-agentic-access
source_filename: root-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/root-platform-api-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 198\n  by_action_class:\n    acting: 128\n    connected: 70\n  by_consequence:\n    write: 100\n    read: 70\n    physical: 27\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /applications\n  method: post\n  operationId: create-application\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications\n  method: get\n  operationId: fetch-applications\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application_id}\n  method: get\n  operationId: retrieve-an-application\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application_id}\n  method: put\n  operationId: requote-application\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application_id}/alteration-packages\n  method: post\n  operationId: create-application-alteration-package\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application_id}/alteration-packages/{alteration_package_id}\n  method: get\n  operationId: retrieve-application-alteration-package\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application_id}/alteration-packages/{alteration_package_id}/apply\n  method: post\n  operationId: apply-application-alteration-package\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application_id}/attachments\n  method: get\n  operationId: retrieve-application-attachments\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application_id}/attachments\n  method: post\n  operationId: add-application-attachments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application_id}/attachments/{attachment_id}/archive\n  method: post\n  operationId: archive-application-attachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application_id}/beneficiaries\n\
  \  method: get\n  operationId: fetch-application-beneficiaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application_id}/beneficiaries\n  method: put\n  operationId: update-application-beneficiaries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application_id}/notes\n  method: get\n  operationId: retrieve-application-notes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application_id}/notes\n  method: post\n  operationId: add-application-notes\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application_id}/events\n  method: get\n  operationId: retrieve-application-events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application_id}/payment-method\n  method: get\n  operationId: retrieve-application-payment-method\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application_id}/payment-method\n  method: post\n  operationId: assign-application-payment-method\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application_id}/send-application-pdf-to-policyholder\n  method: post\n  operationId: send-application-pdf-to-policyholder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application_id}/cancellation-reasons\n  method: get\n  operationId: get-application-cancellation-reasons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{application_id}/cancel\n\
  \  method: post\n  operationId: cancel-application\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{application_id}/archive\n  method: post\n  operationId: archive-application\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /organizations/{client_app_id}/applications/{application_id}/alteration-hooks\n  method: get\n  operationId: retrieve-application-alteration-hooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /calls\n  method: get\n  operationId: fetch-calls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calls\n  method: post\n  operationId: create-call\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /calls/{call_id}\n  method: get\n  operationId: retrieve-call\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /calls/{call_id}/events\n  method: get\n  operationId: retrieve-call-events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /calls/{call_id}/playback-url\n  method: get\n  operationId: retrieve-call-playback-url\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /claims\n  method: post\n  operationId: create-claim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claims\n  method: get\n  operationId: fetch-claims\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /claims/{claim_id}\n  method: get\n  operationId: retrieve-a-claim\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /claims/{claim_id}\n  method: patch\n  operationId: updating-a-claim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claims/{claim_id}/acknowledge-approved\n  method: post\n  operationId: acknowledge-approved\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claims/{claim_id}/acknowledge-goodwill\n  method: post\n  operationId: acknowledge-goodwill\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claims/{claim_id}/acknowledge-no-claim\n  method: post\n  operationId: acknowledge-no-claim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claims/{claim_id}/acknowledge-repudiated\n  method: post\n  operationId: acknowledge-repudiated\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claims/{claim_id}/approve\n  method: post\n  operationId: approve-claim\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claims/{claim_id}/attachments\n  method: get\n  operationId: retrieve-claim-attachments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /claims/{claim_id}/attachments\n  method: post\n  operationId: claim-create-attachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claims/{claim_id}/attachments/{attachment_id}/archive\n  method: post\n  operationId: claim-archive-attachment\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claims/{claim_id}/blocks\n  method: patch\n  operationId: update-multiple-block-states\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claims/{claim_id}/block-states/{block_key}\n  method: get\n  operationId: retrieve-a-block-state\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /claims/{claim_id}/blocks/{block_key}\n  method: patch\n  operationId: updating-a-block-state\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claims/{claim_id}/do-not-acknowledge-approved\n  method: post\n  operationId: do-not-acknowledge-approved\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claims/{claim_id}/do-not-acknowledge-goodwill\n  method: post\n  operationId: do-not-acknowledge-goodwill\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /claims/{claim_id}/do-not-acknowledge-no-claim\n  method: post\n  operationId: do-not-acknowledge-no-claim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claims/{claim_id}/do-not-acknowledge-repudiated\n  method: post\n  operationId: do-not-acknowledge-repudiated\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claims/{claim_id}/goodwill\n  method: post\n  operationId: goodwill-claim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claims/{claim_id}/no-claim\n  method: post\n  operationId: no-claim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claims/{claim_id}/notes\n  method: get\n  operationId: retrieve-claim-notes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /claims/{claim_id}/notes\n  method: post\n  operationId: claim-add-note\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claims/{claim_id}/policy\n  method: post\n  operationId: claim-link-policy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claims/fulfillment-requests/{fulfillment_request_id}/approve\n  method: patch\n  operationId: approve-fulfillment-request\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claims/fulfillment-requests/{fulfillment_request_id}/reject\n\
  \  method: patch\n  operationId: reject-a-fulfillment-request\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claims/{claim_id}/repudiate\n  method: post\n  operationId: repudiate-claim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claims/{claim_id}/send-to-review\n  method: post\n  operationId: send-to-review\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n  \
  \    exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claims/{claim_id}/close\n  method: post\n  operationId: close-claim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claims/{claim_id}/reopen\n  method: post\n  operationId: reopen-claim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claims/{claim_id}/claimant\n  method: patch\n  operationId: update-claimant\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claims/{claim_id}/events\n  method: get\n  operationId: get-claim-events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /claims/{claim_id}/paid-out\n  method: post\n  operationId: paid-out-claim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /claims/{claim_id}/send-to-capture\n  method: post\n  operationId: send-to-capture\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /complaints\n  method: post\n  operationId: create-a-complaint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /complaints\n  method: get\n  operationId: list-all-complaints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /complaints/{complaint_id}\n  method: get\n  operationId: retrieve-a-complaint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n \
  \   subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /complaints/{complaint_id}\n  method: patch\n  operationId: update-complaint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /complaints/{complaint_id}/attachments\n  method: get\n  operationId: retrieve-complaint-attachments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /complaints/{complaint_id}/attachments\n  method: post\n  operationId: complaint-create-attachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /complaints/{complaint_id}/attachments/{attachment_id}/archive\n  method: post\n  operationId: complaint-archive-attachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /complaints/{complaint_id}/close\n  method: post\n  operationId: close-complaint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /complaints/{complaint_id}/events\n  method: get\n  operationId: get-complaint-events\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /complaints/{complaint_id}/complainant\n  method: patch\n  operationId: complaint-update-complainant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /complaints/{complaint_id}/notes\n  method: get\n  operationId: fetch-complaint-notes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /complaints/{complaint_id}/notes\n  method: post\n  operationId: complaint-create-note\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /complaints/{complaint_id}/policy\n  method: post\n  operationId: complaint-link-policy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /complaints/{complaint_id}/reopen\n  method: post\n  operationId: reopen-complaint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /custom-notification-events/{custom_event_key}/trigger\n  method: post\n  operationId: trigger-custom-notification-event\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data-export-runs\n  method: get\n  operationId: fetch-data-export-runs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data-export-runs/{data_export_run_id}\n  method: get\n  operationId: retrieve-data-export-run\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data-export-runs/{data_export_run_id}/log-items\n  method: get\n  operationId: fetch-data-export-run-log\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data-stores\n\
  \  method: get\n  operationId: list-data-stores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data-stores\n  method: post\n  operationId: create-data-store\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data-stores/{data_store_key}/entities\n  method: head\n  operationId: count-data-store-entities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data-stores/{data_store_key}/entities\n  method: get\n  operationId: list-data-store-entities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /data-stores/{data_store_key}/entities\n  method: post\n  operationId: create-data-store-entity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data-stores/{data_store_key}\n  method: get\n  operationId: retrieve-data-store\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data-stores/{data_store_key}\n  method: delete\n  operationId: archive-data-store\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n     \
  \ - high-value\n    audit: required\n- path: /data-stores/{data_store_key}\n  method: patch\n  operationId: update-data-store\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data-stores/{data_store_key}/entities/{data_store_entity_id}\n  method: delete\n  operationId: archive-data-store-entity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data-stores/{data_store_key}/entities/{data_store_entity_id}\n  method: get\n  operationId: retrieve-data-store-entity\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data-stores/{data_store_key}/entities/{data_store_entity_id}\n  method: patch\n  operationId: update-data-store-entity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leads\n  method: get\n  operationId: fetch-leads\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /leads\n  method: post\n  operationId: create-lead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /leads\n  method: put\n  operationId: create-or-update-lead\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /leads/archive\n  method: post\n  operationId: archive-leads\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /notifications\n  method: get\n  operationId: fetch-notifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notifications\n  method: post\n  operationId: create-external-notification\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /notifications/{notification_id}\n  method: get\n  operationId: retrieve-a-notification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notifications/{notification_id}\n  method: patch\n  operationId: update-external-notification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment-batches/{payment_batch_id}\n  method: patch\n  operationId: update-payment-batch\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/async-create\n  method: post\n  operationId: async-payments-create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/async-update\n  method: post\n  operationId: update-payments-async\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      trigg\n\n# --- truncated at 32 KB (63 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/root/refs/heads/main/agentic-access/root-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/root/refs/heads/main/agentic-access/root-agentic-access.yml
summary_line: 198 operations · 128 acting · 1 human-in-the-loop
tags:
- Insurance
- Auto Insurance
- Telematics
- Embedded Insurance
- Policy Administration
- Claims
- Usage-Based Insurance
- InsurTech
---
