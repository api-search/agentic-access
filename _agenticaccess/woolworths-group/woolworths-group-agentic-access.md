---
acting_count: 21
action_class_counts:
  acting: 21
  connected: 29
api_specs:
- filename: woolworths-group-accountstatusinquiry-api-openapi.yml
  format: yaml
  label: Woolworths Group Account Status Inquiry API
  slug: woolworths-group-accountstatusinquiry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woolworths-group/refs/heads/main/openapi/woolworths-group-accountstatusinquiry-api-openapi.yml
- filename: woolworths-group-activating-physical-gift-cards-api-openapi.yml
  format: yaml
  label: Woolworths Group Activating Physical Gift Cards API
  slug: woolworths-group-activating-physical-gift-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woolworths-group/refs/heads/main/openapi/woolworths-group-activating-physical-gift-cards-api-openapi.yml
- filename: woolworths-group-authorization-api-openapi.yml
  format: yaml
  label: Woolworths Group Authorization API
  slug: woolworths-group-authorization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woolworths-group/refs/heads/main/openapi/woolworths-group-authorization-api-openapi.yml
- filename: woolworths-group-capture-api-openapi.yml
  format: yaml
  label: Woolworths Group Capture API
  slug: woolworths-group-capture-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woolworths-group/refs/heads/main/openapi/woolworths-group-capture-api-openapi.yml
- filename: woolworths-group-gifting-catalogue-api-openapi.yml
  format: yaml
  label: Woolworths Group Gifting Catalogue API
  slug: woolworths-group-gifting-catalogue-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woolworths-group/refs/heads/main/openapi/woolworths-group-gifting-catalogue-api-openapi.yml
- filename: woolworths-group-health-check-api-openapi.yml
  format: yaml
  label: Woolworths Group Health check API
  slug: woolworths-group-health-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woolworths-group/refs/heads/main/openapi/woolworths-group-health-check-api-openapi.yml
- filename: woolworths-group-instruments-api-openapi.yml
  format: yaml
  label: Woolworths Group Instruments API
  slug: woolworths-group-instruments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woolworths-group/refs/heads/main/openapi/woolworths-group-instruments-api-openapi.yml
- filename: woolworths-group-key-management-api-openapi.yml
  format: yaml
  label: Woolworths Group Key Management API
  slug: woolworths-group-key-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woolworths-group/refs/heads/main/openapi/woolworths-group-key-management-api-openapi.yml
- filename: woolworths-group-order-api-openapi.yml
  format: yaml
  label: Woolworths Group Order API
  slug: woolworths-group-order-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woolworths-group/refs/heads/main/openapi/woolworths-group-order-api-openapi.yml
- filename: woolworths-group-ordering-digital-gift-cards-api-openapi.yml
  format: yaml
  label: Woolworths Group Ordering Digital Gift Cards API
  slug: woolworths-group-ordering-digital-gift-cards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woolworths-group/refs/heads/main/openapi/woolworths-group-ordering-digital-gift-cards-api-openapi.yml
- filename: woolworths-group-payments-api-openapi.yml
  format: yaml
  label: Woolworths Group Payments API
  slug: woolworths-group-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woolworths-group/refs/heads/main/openapi/woolworths-group-payments-api-openapi.yml
- filename: woolworths-group-refund-api-openapi.yml
  format: yaml
  label: Woolworths Group Refund API
  slug: woolworths-group-refund-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woolworths-group/refs/heads/main/openapi/woolworths-group-refund-api-openapi.yml
- filename: woolworths-group-refunds-api-openapi.yml
  format: yaml
  label: Woolworths Group Refunds API
  slug: woolworths-group-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woolworths-group/refs/heads/main/openapi/woolworths-group-refunds-api-openapi.yml
- filename: woolworths-group-support-api-openapi.yml
  format: yaml
  label: Woolworths Group Support API
  slug: woolworths-group-support-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woolworths-group/refs/heads/main/openapi/woolworths-group-support-api-openapi.yml
- filename: woolworths-group-transaction-api-openapi.yml
  format: yaml
  label: Woolworths Group Transaction API
  slug: woolworths-group-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woolworths-group/refs/heads/main/openapi/woolworths-group-transaction-api-openapi.yml
- filename: woolworths-group-void-api-openapi.yml
  format: yaml
  label: Woolworths Group Void API
  slug: woolworths-group-void-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woolworths-group/refs/heads/main/openapi/woolworths-group-void-api-openapi.yml
- filename: woolworths-group-wallet-services-api-openapi.yml
  format: yaml
  label: Woolworths Group Wallet Services API
  slug: woolworths-group-wallet-services-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/woolworths-group/refs/heads/main/openapi/woolworths-group-wallet-services-api-openapi.yml
consequence_counts:
  physical: 9
  read: 29
  write: 12
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Woolworths Group Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/v1/transactions/{transactionId}/refunds/{refundId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /gco/client/api/v1/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /gco/client/api/v1/orders/{clientOrderNumber}/items/fulfillment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /merchants/{merchantId}/instruments/{instrumentId}/payment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /merchants/{merchantId}/payments/{paymentId}/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /merchants/{merchantId}/session/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /merchants/{merchantId}/session/payment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /orders/reverse
operation_count: 50
overview: 'Woolworths Group exposes 50 API operations that an AI agent could call, of which 21 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 29 read, 12 write, and 9 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Woolworths Group
provider_slug: woolworths-group
slug: woolworths-group-agentic-access
source_filename: woolworths-group-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-22'\nmethod: generated\nsource: openapi/woolworths-group-wpay-cards-connect-openapi.yml, openapi/woolworths-group-wpay-gift-card-partner-openapi.yml,\n  openapi/woolworths-group-wpay-gifting-client-openapi.yml, openapi/woolworths-group-wpay-payment-openapi.yml,\n  openapi/woolworths-group-wpay-payto-merchant-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 50\n  by_action_class:\n    acting: 21\n    connected: 29\n  by_consequence:\n    write: 12\n    read: 29\n    physical: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/transactions/{transactionId}/captures/{captureId}\n  method: put\n  operationId: CaptureAuthorizationAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/transactions/{transactionId}/captures/{captureId}\n  method: get\n  operationId: GetCaptureAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/account-status-inquiries/{id}\n  method: put\n  operationId: CreateAccountStatusInquiryAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/account-status-inquiries/{id}\n  method: get\n  operationId: GetAccountStatusInquiryAsync\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/transactions/{transactionId}/authorization\n  method: put\n  operationId: CreateAuthorizationAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/transactions/{transactionId}/authorization\n  method: get\n  operationId: GetAuthorizationAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/transactions/{transactionId}/captures\n  method: get\n  operationId: GetCapturesAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/v1/keys/credential/{keyId}/public\n  method: get\n  operationId: GetCredentialPublicKeyAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/keys/current/public\n  method: get\n  operationId: GetPublicKeyAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/keys/{keyId}/public\n  method: get\n  operationId: GetPublicKeyByIdAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/transactions/{transactionId}/refunds/{refundId}\n  method: get\n  operationId: GetRefundAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/transactions/{transactionId}/refunds/{refundId}\n\
  \  method: put\n  operationId: RefundAuthorizationAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/transactions/{transactionId}/refunds\n  method: get\n  operationId: GetRefundsAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/transactions/{transactionId}\n  method: get\n  operationId: GetTransactionAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/transactions/{transactionId}/voids/{voidId}\n  method: get\n  operationId: GetVoidAsync\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/transactions/{transactionId}/voids/{voidId}\n  method: put\n  operationId: VoidAuthorizationAsync\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/transactions/{transactionId}/voids\n  method: get\n  operationId: GetVoidsAsync\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/keys/credential/rotate-to/{keyId}\n  method: put\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /activations/physical\n  method: post\n  operationId: activatePhysicalGiftCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /order/{orderId}/cards\n  method: get\n  operationId: getActivatedGiftCards\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /order/{refno}/status\n  method: get\n  operationId: getGiftCardOrderStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /health\n  method: get\n  operationId: getServiceHealth\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /orders\n  method: post\n  operationId: orderGiftCards\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /orders/reverse\n  method: post\n  operationId: postOrdersReverse\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gco/client/api/v1/orders/{clientOrderNumber}/items/fulfillment\n\
  \  method: post\n  operationId: ClientReAttemptDelivery\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gcc/client/api/v1/catalogue/products\n  method: get\n  operationId: GetAllProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gcc/client/api/v1/catalogue/programs\n  method: get\n  operationId: GetAllPrograms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gcc/client/api/v1/catalogue/categories\n  method: get\n  operationId: GetCategories\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gcc/client/api/v1/catalogue/categories/{id}\n  method: get\n  operationId: GetCategoryById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gco/client/api/v1/orders/{clientOrderNumber}/details\n  method: get\n  operationId: GetOrderDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gco/client/api/v1/orders/{clientOrderNumber}/status\n  method: get\n  operationId: GetOrderStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gcc/client/api/v1/catalogue/products/{id}\n  method: get\n  operationId: GetProductById\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gcc/client/api/v1/catalogue/programs/{id}\n  method: get\n  operationId: GetProgramById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gco/client/api/v1/orders\n  method: post\n  operationId: SubmitOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /cancel\n  method: post\n  operationId: cancel-transaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n    \
  \  human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api-key\n  method: post\n  operationId: create-key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api-key\n  method: get\n  operationId: get-keys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction\n  method: post\n  operationId: create-transaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /api-key/{keyId}\n  method: delete\n  operationId: delete-key\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merchants/{merchantId}/buyers/{buyerId}/instruments\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchants/{merchantId}/instruments/{instrumentId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchants/{merchantId}/payments/{paymentId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /merchants/{merchantId}/refunds/{refundId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchants/{merchantId}/sessions/{sessionId}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchants/{merchantId}/instruments/{instrumentId}/cancel\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merchants/{merchantId}/instruments/{instrumentId}/payment\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n  \
  \  token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merchants/{merchantId}/payments/{paymentId}/refund\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merchants/{merchantId}/session/checkout\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /merchants/{merchantId}/session/instrument\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /merchants/{merchantId}/session/payment\n  method: post\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/woolworths-group/refs/heads/main/agentic-access/woolworths-group-agentic-access.yml
summary_line: 50 operations · 21 acting
tags:
- Company
- Retail
- Supermarkets
- Grocery
- Australia
- New Zealand
- E-Commerce
---
