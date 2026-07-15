---
acting_count: 371
action_class_counts:
  acting: 371
  connected: 963
api_specs:
- filename: openapi.json
  format: json
  label: Commerce Layer Core API
  slug: commerce-layer-core-api
  spec_type: OpenAPI
  url: https://data.commercelayer.app/schemas/openapi.json
- filename: openapi.json
  format: json
  label: Commerce Layer Provisioning API
  slug: commerce-layer-provisioning-api
  spec_type: OpenAPI
  url: https://data.commercelayer.app/schemas/provisioning/openapi.json
- filename: openapi.json
  format: json
  label: Commerce Layer Metrics API
  slug: commerce-layer-metrics-api
  spec_type: OpenAPI
  url: https://data.commercelayer.app/schemas/metrics/openapi.json
consequence_counts:
  physical: 98
  read: 963
  safety-critical: 3
  write: 270
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Commerce Layer Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /customer_password_resets
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /customer_password_resets/{customerPasswordResetId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /customer_password_resets/{customerPasswordResetId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /adyen_payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /adyen_payments/{adyenPaymentId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /adyen_payments/{adyenPaymentId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /application_memberships
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /application_memberships/{applicationMembershipId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /application_memberships/{applicationMembershipId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /axerve_payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /axerve_payments/{axervePaymentId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /axerve_payments/{axervePaymentId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /braintree_payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /braintree_payments/{braintreePaymentId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /braintree_payments/{braintreePaymentId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout_com_gateways
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /checkout_com_gateways/{checkoutComGatewayId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /checkout_com_gateways/{checkoutComGatewayId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /checkout_com_payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /checkout_com_payments/{checkoutComPaymentId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /checkout_com_payments/{checkoutComPaymentId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /customer_payment_sources
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /customer_payment_sources/{customerPaymentSourceId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /customer_payment_sources/{customerPaymentSourceId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /external_payments
operation_count: 1334
overview: 'Commerce Layer exposes 1334 API operations that an AI agent could call, of which 371 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 963 read, 270 write, 98 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Commerce Layer
provider_slug: commerce-layer
slug: commerce-layer-agentic-access
source_filename: commerce-layer-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/commerce-layer-core-api-openapi.json, openapi/commerce-layer-metrics-api-openapi.json,\n  openapi/commerce-layer-provisioning-api-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 1334\n  by_action_class:\n    connected: 963\n    acting: 371\n  by_consequence:\n    read: 963\n    write: 270\n    physical: 98\n    safety-critical: 3\n  human_in_the_loop_required: 3\noperations:\n- path: /addresses\n  method: get\n  operationId: GET/addresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /addresses\n  method: post\n  operationId: POST/addresses\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /addresses/{addressId}\n  method: get\n  operationId: GET/addresses/addressId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /addresses/{addressId}\n  method: patch\n  operationId: PATCH/addresses/addressId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /addresses/{addressId}\n  method: delete\n  operationId: DELETE/addresses/addressId\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /addresses/{addressId}/geocoder\n  method: get\n  operationId: GET/addressId/geocoder\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /addresses/{addressId}/events\n  method: get\n  operationId: GET/addressId/events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /addresses/{addressId}/tags\n  method: get\n  operationId: GET/addressId/tags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /addresses/{addressId}/event_stores\n  method: get\n\
  \  operationId: GET/addressId/event_stores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /adjustments\n  method: get\n  operationId: GET/adjustments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /adjustments\n  method: post\n  operationId: POST/adjustments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /adjustments/{adjustmentId}\n  method: get\n  operationId: GET/adjustments/adjustmentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /adjustments/{adjustmentId}\n  method: patch\n  operationId: PATCH/adjustments/adjustmentId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /adjustments/{adjustmentId}\n  method: delete\n  operationId: DELETE/adjustments/adjustmentId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /adjustments/{adjustmentId}/event_stores\n  method: get\n  operationId: GET/adjustmentId/event_stores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /adyen_gateways\n  method: get\n  operationId: GET/adyen_gateways\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /adyen_gateways\n  method: post\n  operationId: POST/adyen_gateways\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /adyen_gateways/{adyenGatewayId}\n  method: get\n  operationId: GET/adyen_gateways/adyenGatewayId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /adyen_gateways/{adyenGatewayId}\n  method: patch\n  operationId: PATCH/adyen_gateways/adyenGatewayId\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /adyen_gateways/{adyenGatewayId}\n  method: delete\n  operationId: DELETE/adyen_gateways/adyenGatewayId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /adyen_gateways/{adyenGatewayId}/payment_methods\n  method: get\n  operationId: GET/adyenGatewayId/payment_methods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /adyen_gateways/{adyenGatewayId}/event_stores\n  method: get\n  operationId: GET/adyenGatewayId/event_stores\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /adyen_gateways/{adyenGatewayId}/adyen_payments\n  method: get\n  operationId: GET/adyenGatewayId/adyen_payments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /adyen_payments\n  method: get\n  operationId: GET/adyen_payments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /adyen_payments\n  method: post\n  operationId: POST/adyen_payments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /adyen_payments/{adyenPaymentId}\n  method: get\n  operationId: GET/adyen_payments/adyenPaymentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /adyen_payments/{adyenPaymentId}\n  method: patch\n  operationId: PATCH/adyen_payments/adyenPaymentId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /adyen_payments/{adyenPaymentId}\n  method: delete\n  operationId: DELETE/adyen_payments/adyenPaymentId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /adyen_payments/{adyenPaymentId}/order\n  method: get\n  operationId: GET/adyenPaymentId/order\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /adyen_payments/{adyenPaymentId}/payment_gateway\n  method: get\n  operationId: GET/adyenPaymentId/payment_gateway\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /adyen_payments/{adyenPaymentId}/event_stores\n  method: get\n  operationId: GET/adyenPaymentId/event_stores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /application\n  method: get\n  operationId: GET/application/applicationId\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attachments\n  method: get\n  operationId: GET/attachments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attachments\n  method: post\n  operationId: POST/attachments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /attachments/{attachmentId}\n  method: get\n  operationId: GET/attachments/attachmentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /attachments/{attachmentId}\n  method:\
  \ patch\n  operationId: PATCH/attachments/attachmentId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /attachments/{attachmentId}\n  method: delete\n  operationId: DELETE/attachments/attachmentId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /attachments/{attachmentId}/event_stores\n  method: get\n  operationId: GET/attachmentId/event_stores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorizations\n  method:\
  \ get\n  operationId: GET/authorizations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorizations/{authorizationId}\n  method: get\n  operationId: GET/authorizations/authorizationId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorizations/{authorizationId}\n  method: patch\n  operationId: PATCH/authorizations/authorizationId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /authorizations/{authorizationId}/order\n  method: get\n  operationId: GET/authorizationId/order\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorizations/{authorizationId}/attachments\n  method: get\n  operationId: GET/authorizationId/attachments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorizations/{authorizationId}/events\n  method: get\n  operationId: GET/authorizationId/events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorizations/{authorizationId}/event_stores\n  method: get\n  operationId: GET/authorizationId/event_stores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorizations/{authorizationId}/captures\n  method: get\n  operationId: GET/authorizationId/captures\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authorizations/{authorizationId}/voids\n  method: get\n  operationId: GET/authorizationId/voids\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /avalara_accounts\n  method: get\n  operationId: GET/avalara_accounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /avalara_accounts\n  method: post\n  operationId: POST/avalara_accounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /avalara_accounts/{avalaraAccountId}\n\
  \  method: get\n  operationId: GET/avalara_accounts/avalaraAccountId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /avalara_accounts/{avalaraAccountId}\n  method: patch\n  operationId: PATCH/avalara_accounts/avalaraAccountId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /avalara_accounts/{avalaraAccountId}\n  method: delete\n  operationId: DELETE/avalara_accounts/avalaraAccountId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /avalara_accounts/{avalaraAccountId}/markets\n  method: get\n  operationId: GET/avalaraAccountId/markets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /avalara_accounts/{avalaraAccountId}/attachments\n  method: get\n  operationId: GET/avalaraAccountId/attachments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /avalara_accounts/{avalaraAccountId}/events\n  method: get\n  operationId: GET/avalaraAccountId/events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /avalara_accounts/{avalaraAccountId}/event_stores\n  method: get\n  operationId: GET/avalaraAccountId/event_stores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /avalara_accounts/{avalaraAccountId}/tax_categories\n  method: get\n  operationId: GET/avalaraAccountId/tax_categories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /axerve_gateways\n  method: get\n  operationId: GET/axerve_gateways\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /axerve_gateways\n  method: post\n  operationId: POST/axerve_gateways\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /axerve_gateways/{axerveGatewayId}\n  method: get\n  operationId: GET/axerve_gateways/axerveGatewayId\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /axerve_gateways/{axerveGatewayId}\n  method: patch\n  operationId: PATCH/axerve_gateways/axerveGatewayId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /axerve_gateways/{axerveGatewayId}\n  method: delete\n  operationId: DELETE/axerve_gateways/axerveGatewayId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /axerve_gateways/{axerveGatewayId}/payment_methods\n  method:\
  \ get\n  operationId: GET/axerveGatewayId/payment_methods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /axerve_gateways/{axerveGatewayId}/event_stores\n  method: get\n  operationId: GET/axerveGatewayId/event_stores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /axerve_gateways/{axerveGatewayId}/axerve_payments\n  method: get\n  operationId: GET/axerveGatewayId/axerve_payments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /axerve_payments\n  method: get\n  operationId: GET/axerve_payments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /axerve_payments\n  method:\
  \ post\n  operationId: POST/axerve_payments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /axerve_payments/{axervePaymentId}\n  method: get\n  operationId: GET/axerve_payments/axervePaymentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /axerve_payments/{axervePaymentId}\n  method: patch\n  operationId: PATCH/axerve_payments/axervePaymentId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /axerve_payments/{axervePaymentId}\n  method: delete\n  operationId: DELETE/axerve_payments/axervePaymentId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /axerve_payments/{axervePaymentId}/order\n  method: get\n  operationId: GET/axervePaymentId/order\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /axerve_payments/{axervePaymentId}/payment_gateway\n  method: get\n  operationId: GET/axervePaymentId/payment_gateway\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /axerve_payments/{axervePaymentId}/event_stores\n  method: get\n  operationId: GET/axervePaymentId/event_stores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bing_geocoders\n  method: get\n  operationId: GET/bing_geocoders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bing_geocoders\n  method: post\n  operationId: POST/bing_geocoders\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bing_geocoders/{bingGeocoderId}\n  method: get\n  operationId: GET/bing_geocoders/bingGeocoderId\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bing_geocoders/{bingGeocoderId}\n  method: patch\n  operationId: PATCH/bing_geocoders/bingGeocoderId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bing_geocoders/{bingGeocoderId}\n  method: delete\n  operationId: DELETE/bing_geocoders/bingGeocoderId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bing_geocoders/{bingGeocoderId}/markets\n  method: get\n  operationId:\
  \ GET/bingGeocoderId/markets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bing_geocoders/{bingGeocoderId}/addresses\n  method: get\n  operationId: GET/bingGeocoderId/addresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bing_geocoders/{bingGeocoderId}/attachments\n  method: get\n  operationId: GET/bingGeocoderId/attachments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bing_geocoders/{bingGeocoderId}/event_stores\n  method: get\n  operationId: GET/bingGeocoderId/event_stores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /braintree_gateways\n  method: get\n\
  \  operationId: GET/braintree_gateways\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /braintree_gateways\n  method: post\n  operationId: POST/braintree_gateways\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /braintree_gateways/{braintreeGatewayId}\n  method: get\n  operationId: GET/braintree_gateways/braintreeGatewayId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /braintree_gateways/{braintreeGatewayId}\n  method: patch\n  operationId: PATCH/braintree_gateways/braintreeGatewayId\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /braintree_gateways/{braintreeGatewayId}\n  method: delete\n  operationId: DELETE/braintree_gateways/braintreeGatewayId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /braintree_gateways/{braintreeGatewayId}/payment_methods\n  method: get\n  operationId: GET/braintreeGatewayId/payment_methods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /braintree_gateways/{braintreeGatewayId}/event_stores\n  method: get\n  operationId: GET/braintreeGatewayId/event_stores\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /braintree_gateways/{braintreeGatewayId}/braintree_payments\n  method: get\n  operationId: GET/braintreeGatewayId/braintree_payments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /braintree_payments\n  method: get\n  operationId: GET/braintree_payments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /braintree_payments\n  method: post\n  operationId: POST/braintree_payments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /braintree_payments/{braintreePaymentId}\n  method: get\n  operationId: GET/braintree_payments/braintreePaymentId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /braintree_payments/{braintreePaymentId}\n  method: patch\n  operationId: PATCH/braintree_payments/braintreePaymentId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /braintree_payments/{braintreePaymentId}\n  method: delete\n  operationId: DELETE/braintree_payments/braintreePaymentId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /braintree_payments/{braintreePaymentId}/order\n  method: get\n  operationId: GET/braintreePaymentId/order\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /braintree_payments/{braintreePaymentId}/payment_gateway\n  method: get\n  operationId: GET/braintreePaymentId/payment_gateway\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /braintree_payments/{braintreePaymentId}/event_stores\n  method: get\n  operationId: GET/braintreePaymentId/event_stores\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bundles\n  method: get\n  operationId: GET/bundles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bundles\n  method: post\n  operationId: POST/bundles\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bundles/{bundleId}\n  method: get\n  operationId: GET/bundles/bundleId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bundles/{bundleId}\n  method: patch\n  operationId: PATCH/bundles/bundleId\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bundles/{bundleId}\n  method: delete\n  operationId: DELETE/bundles/bundleId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bundles/{bundleId}/market\n  method: get\n  operationId: GET/bundleId/market\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bundles/{bundleId}/sku_list\n  method: get\n  operationId: GET/bundleId/sku_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /bundles/{bundleId}/skus\n  method: get\n  operationId: GET/bundleId/skus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bundles/{bundleId}/attachments\n  method: get\n  operationId: GET/bundleId/attachments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bundles/{bundleId}/events\n  method: get\n  operationId: GET/bundleId/events\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bundles/{bundleId}/tags\n  method: get\n  operationId: GET/bundleId/tags\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bundles/{bundleId}/event_stores\n\
  \  method: get\n  operationId: GET/bundleId/event_stores\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /buy_x_pay_y_promotions\n  method: get\n  operationId: GET/buy_x_pay_y_promotions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /buy_x_pay_y_promotions\n  method: post\n  operationId: POST/buy_x_pay_y_promotions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /buy_x_pay_y_promotions/{buyXPayYPromotionId}\n  method: get\n  operationId: GET/buy_x_pay_y_promotions/buyXPayYPromotionId\n  x-agentic-access:\n    action-class: connecte\n\n# ---\
  \ truncated at 32 KB (370 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/commerce-layer/refs/heads/main/agentic-access/commerce-layer-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/commerce-layer/refs/heads/main/agentic-access/commerce-layer-agentic-access.yml
summary_line: 1334 operations · 371 acting · 3 human-in-the-loop
tags:
- Headless Commerce
- Composable Commerce
- API-First
- Ecommerce
- JSON:API
- OAuth 2.0
- Multi-Market
- Multi-Currency
- B2C
- B2B
- Subscriptions
- Promotions
- Inventory
- Order Management
- Checkout
---
