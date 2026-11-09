---
acting_count: 35
action_class_counts:
  acting: 35
  connected: 67
api_specs:
- filename: payments-ai-api-keys-api-openapi.yml
  format: yaml
  label: payments-ai API Keys API
  slug: payments-ai-api-keys-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/payments-ai/openapi/payments-ai-api-keys-api-openapi.yml
- filename: payments-ai-buyer-checkout-api-openapi.yml
  format: yaml
  label: payments-ai Buyer checkout API
  slug: payments-ai-buyer-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/payments-ai/openapi/payments-ai-buyer-checkout-api-openapi.yml
- filename: payments-ai-checkout-api-openapi.yml
  format: yaml
  label: payments-ai Checkout API
  slug: payments-ai-checkout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/payments-ai/openapi/payments-ai-checkout-api-openapi.yml
- filename: payments-ai-customers-api-openapi.yml
  format: yaml
  label: payments-ai Customers API
  slug: payments-ai-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/payments-ai/openapi/payments-ai-customers-api-openapi.yml
- filename: payments-ai-invoices-api-openapi.yml
  format: yaml
  label: payments-ai Invoices API
  slug: payments-ai-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/payments-ai/openapi/payments-ai-invoices-api-openapi.yml
- filename: payments-ai-json-api-openapi.yml
  format: yaml
  label: payments-ai JSON API
  slug: payments-ai-json-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/payments-ai/openapi/payments-ai-json-api-openapi.yml
- filename: payments-ai-markdown-api-openapi.yml
  format: yaml
  label: payments-ai Markdown API
  slug: payments-ai-markdown-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/payments-ai/openapi/payments-ai-markdown-api-openapi.yml
- filename: payments-ai-merchant-api-openapi.yml
  format: yaml
  label: payments-ai Merchant API
  slug: payments-ai-merchant-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/payments-ai/openapi/payments-ai-merchant-api-openapi.yml
- filename: payments-ai-orders-api-openapi.yml
  format: yaml
  label: payments-ai Orders API
  slug: payments-ai-orders-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/payments-ai/openapi/payments-ai-orders-api-openapi.yml
- filename: payments-ai-pages-api-openapi.yml
  format: yaml
  label: payments-ai Pages API
  slug: payments-ai-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/payments-ai/openapi/payments-ai-pages-api-openapi.yml
- filename: payments-ai-products-api-openapi.yml
  format: yaml
  label: payments-ai Products API
  slug: payments-ai-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/payments-ai/openapi/payments-ai-products-api-openapi.yml
- filename: payments-ai-public-api-api-openapi.yml
  format: yaml
  label: payments-ai Public API
  slug: payments-ai-public-api-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/payments-ai/openapi/payments-ai-public-api-api-openapi.yml
- filename: payments-ai-subscriptions-api-openapi.yml
  format: yaml
  label: payments-ai Subscriptions API
  slug: payments-ai-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/payments-ai/openapi/payments-ai-subscriptions-api-openapi.yml
- filename: payments-ai-transactions-api-openapi.yml
  format: yaml
  label: payments-ai Transactions API
  slug: payments-ai-transactions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/payments-ai/openapi/payments-ai-transactions-api-openapi.yml
consequence_counts:
  physical: 17
  read: 67
  safety-critical: 1
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Payments Ai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/public-api/merchants/{merchantId}/api-keys/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/checkout/orders/{orderId}/confirm
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/checkout/orders/{orderId}/promo-code-preview
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/checkout/orders/{orderId}/tax
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/checkout/plans/{planId}/confirm
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/checkout/plans/{planId}/promo-code-preview
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/checkout/plans/{planId}/promo-codes
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/checkout/plans/{planId}/session
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/checkout/plans/{planId}/tax
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/public-api/merchants/{merchantId}/checkout/customization
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/public-api/merchants/{merchantId}/checkout/logo/confirm
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/public-api/merchants/{merchantId}/checkout/logo/upload-url
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/public-api/merchants/{merchantId}/checkout/plans/{planId}/confirm
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/public-api/merchants/{merchantId}/checkout/plans/{planId}/promo-code-preview
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/public-api/merchants/{merchantId}/checkout/plans/{planId}/promo-codes
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/public-api/merchants/{merchantId}/checkout/plans/{planId}/session
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/public-api/merchants/{merchantId}/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/public-api/merchants/{merchantId}/payouts
operation_count: 102
overview: 'payments-ai exposes 102 API operations that an AI agent could call, of which 35 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 67 read, 17 write, 17 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: payments-ai
provider_slug: payments-ai
slug: payments-ai-agentic-access
source_filename: payments-ai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/payments-ai-mor-openapi.json, openapi/payments-ai-website-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 102\n  by_action_class:\n    connected: 67\n    acting: 35\n  by_consequence:\n    read: 67\n    physical: 17\n    write: 17\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /v1/checkout/invoices/{invoiceId}\n  method: get\n  operationId: PublicCheckout_getByInvoiceId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/checkout/merchants/{merchantId}/config\n  method: get\n  operationId: PublicCheckout_getMerchantConfig\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/checkout/orders/{orderId}\n  method: get\n  operationId: PublicCheckout_getByOrderId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/checkout/orders/{orderId}/confirm\n  method: post\n  operationId: PublicCheckout_confirmPaymentByOrderId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/checkout/orders/{orderId}/policies/{policyType}\n  method: get\n  operationId: PublicCheckout_redirectPolicyByOrderId\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/checkout/orders/{orderId}/promo-code-preview\n  method: post\n  operationId: PublicCheckout_previewPromoCodeByOrderId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/checkout/orders/{orderId}/receipts/{receiptId}\n  method: get\n  operationId: PublicCheckout_getReceiptByOrderId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/checkout/orders/{orderId}/tax\n  method: post\n  operationId: PublicCheckout_previewTaxByOrderId\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/checkout/plans/{planId}\n  method: get\n  operationId: PublicCheckout_getByPlanId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/checkout/plans/{planId}/confirm\n  method: post\n  operationId: PublicCheckout_confirmPaymentByPlanId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/checkout/plans/{planId}/policies/{policyType}\n\
  \  method: get\n  operationId: PublicCheckout_redirectPolicyByPlanId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/checkout/plans/{planId}/promo-code-preview\n  method: post\n  operationId: PublicCheckout_previewPromoCodeByPlanId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/checkout/plans/{planId}/promo-codes\n  method: post\n  operationId: PublicCheckout_applyPromoCodeByPlanId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n   \
  \ escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/checkout/plans/{planId}/receipts/{receiptId}\n  method: get\n  operationId: PublicCheckout_getReceiptByPlanId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/checkout/plans/{planId}/session\n  method: post\n  operationId: PublicCheckout_createSessionByPlanId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/checkout/plans/{planId}/tax\n  method: post\n  operationId: PublicCheckout_previewTaxByPlanId\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public-api/me/merchants\n  method: get\n  operationId: PublicApiOwnMerchants_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public-api/me/merchants\n  method: post\n  operationId: PublicApiOwnMerchants_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public-api/merchants\n  method: post\n  operationId: PublicApiMerchants_create\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public-api/merchants/{merchantId}\n  method: get\n  operationId: PublicApiMerchants_get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public-api/merchants/{merchantId}\n  method: patch\n  operationId: PublicApiMerchantWebsiteUrl_updateWebsiteUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public-api/merchants/{merchantId}/api-keys\n  method: get\n  operationId: PublicApiApiKeys_list\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public-api/merchants/{merchantId}/api-keys\n  method: post\n  operationId: PublicApiApiKeys_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public-api/merchants/{merchantId}/api-keys/{id}\n  method: delete\n  operationId: PublicApiApiKeys_revoke\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/public-api/merchants/{merchantId}/balances/summary\n\
  \  method: get\n  operationId: PublicApiBalances_summary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public-api/merchants/{merchantId}/checkout/customization\n  method: get\n  operationId: PublicApiCheckoutCustomizationApi_getCustomization\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public-api/merchants/{merchantId}/checkout/customization\n  method: patch\n  operationId: PublicApiCheckoutCustomizationApi_updateCustomization\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public-api/merchants/{merchantId}/checkout/logo/confirm\n\
  \  method: post\n  operationId: PublicApiCheckoutCustomizationApi_confirmLogo\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public-api/merchants/{merchantId}/checkout/logo/upload-url\n  method: post\n  operationId: PublicApiCheckoutCustomizationApi_createLogoUploadUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public-api/merchants/{merchantId}/checkout/plans/{planId}\n  method: get\n  operationId:\
  \ PublicApiCheckout_resolveByPlanId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public-api/merchants/{merchantId}/checkout/plans/{planId}/confirm\n  method: post\n  operationId: PublicApiCheckout_confirmPaymentByPlanId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public-api/merchants/{merchantId}/checkout/plans/{planId}/promo-code-preview\n  method: post\n  operationId: PublicApiCheckout_previewPromoCodeByPlanId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public-api/merchants/{merchantId}/checkout/plans/{planId}/promo-codes\n  method: post\n  operationId: PublicApiCheckout_applyPromoCodeByPlanId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public-api/merchants/{merchantId}/checkout/plans/{planId}/receipts/{receiptId}\n  method: get\n  operationId: PublicApiCheckout_getReceiptByPlanId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public-api/merchants/{merchantId}/checkout/plans/{planId}/session\n\
  \  method: post\n  operationId: PublicApiCheckout_createSessionByPlanId\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public-api/merchants/{merchantId}/customers\n  method: get\n  operationId: PublicApiCustomers_listCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public-api/merchants/{merchantId}/customers/{id}\n  method: get\n  operationId: PublicApiCustomers_getCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public-api/merchants/{merchantId}/discount-codes\n\
  \  method: get\n  operationId: PublicApiDiscountCodes_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public-api/merchants/{merchantId}/discount-codes\n  method: post\n  operationId: PublicApiDiscountCodes_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public-api/merchants/{merchantId}/discount-codes/{id}\n  method: get\n  operationId: PublicApiDiscountCodes_getById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public-api/merchants/{merchantId}/discount-codes/{id}\n  method: patch\n  operationId: PublicApiDiscountCodes_update\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public-api/merchants/{merchantId}/discount-codes/{id}/archive\n  method: post\n  operationId: PublicApiDiscountCodes_archive\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public-api/merchants/{merchantId}/invoices\n  method: get\n  operationId: PublicApiInvoices_listInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public-api/merchants/{merchantId}/invoices/{id}\n\
  \  method: get\n  operationId: PublicApiInvoices_getInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public-api/merchants/{merchantId}/invoices/{id}/download\n  method: get\n  operationId: PublicApiInvoices_downloadInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public-api/merchants/{merchantId}/join-link\n  method: post\n  operationId: PublicApiMerchantJoinLink_remint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public-api/merchants/{merchantId}/members\n  method: post\n  operationId: PublicApiMerchantMembers_assign\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public-api/merchants/{merchantId}/orders\n  method: post\n  operationId: PublicApiOrders_create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public-api/merchants/{merchantId}/orders/{orderId}\n  method: get\n  operationId: PublicApiOrders_getById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public-api/merchants/{merchantId}/payouts\n\
  \  method: post\n  operationId: PublicApiPayouts_requestPayout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public-api/merchants/{merchantId}/payouts/payout-methods\n  method: get\n  operationId: PublicApiPayouts_listPayoutMethods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public-api/merchants/{merchantId}/products\n  method: get\n  operationId: PublicApiProducts_list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public-api/merchants/{merchantId}/products\n  method:\
  \ post\n  operationId: PublicApiProducts_create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public-api/merchants/{merchantId}/products/{id}\n  method: get\n  operationId: PublicApiProducts_getById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public-api/merchants/{merchantId}/products/{id}\n  method: patch\n  operationId: PublicApiProducts_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public-api/merchants/{merchantId}/products/{id}/image/confirm\n\
  \  method: post\n  operationId: PublicApiProducts_confirmImage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public-api/merchants/{merchantId}/products/{id}/image/upload-url\n  method: post\n  operationId: PublicApiProducts_createImageUploadUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public-api/merchants/{merchantId}/products/{id}/plans\n  method: get\n  operationId: PublicApiProducts_listPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v1/public-api/merchants/{merchantId}/products/{id}/plans\n  method: post\n  operationId: PublicApiProducts_createPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public-api/merchants/{merchantId}/products/{id}/plans/{planId}\n  method: patch\n  operationId: PublicApiProducts_updatePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public-api/merchants/{merchantId}/settings/tax\n  method: get\n  operationId: PublicApiMerchantTaxSettingsApi_get\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public-api/merchants/{merchantId}/settings/tax\n  method: patch\n  operationId: PublicApiMerchantTaxSettingsApi_update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public-api/merchants/{merchantId}/subscriptions\n  method: get\n  operationId: PublicApiSubscriptions_listSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public-api/merchants/{merchantId}/subscriptions/{subscriptionId}\n  method: get\n  operationId: PublicApiSubscriptions_getSubscription\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public-api/merchants/{merchantId}/transactions\n  method: post\n  operationId: PublicApiTransactions_createTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/public-api/merchants/{merchantId}/transactions\n  method: get\n  operationId: PublicApiTransactions_listTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/public-api/merchants/{merchantId}/transactions/{id}\n  method: get\n  operationId: PublicApiTransactions_getTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: get\n  operationId: getPageRoot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /index.md\n  method: get\n  operationId: getMarkdownIndexMd\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mor/\n  method: get\n  operationId: getPageMor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mor/index.md\n  method: get\n  operationId: getMarkdownMorIndexMd\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mor/mcp/\n  method: get\n  operationId: getPageMorMcp\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mor/mcp.md\n  method: get\n  operationId: getMarkdownMorMcpMd\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mor/pricing/\n  method: get\n  operationId: getPageMorPricing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mor/pricing.md\n  method: get\n  operationId: getMarkdownMorPricingMd\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platforms/\n  method: get\n  operationId: getPagePlatforms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /platforms/index.md\n  method: get\n  operationId: getMarkdownPlatformsIndexMd\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platforms/pricing/\n  method: get\n  operationId: getPagePlatformsPricing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platforms/pricing.md\n  method: get\n  operationId: getMarkdownPlatformsPricingMd\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /roadmap/\n  method: get\n  operationId: getPageRoadmap\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /roadmap.md\n  method: get\n  operationId: getMarkdownRoadmapMd\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mor/terms-of-service/\n  method: get\n  operationId: getPageMorTermsOfService\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mor/terms-of-service.md\n  method: get\n  operationId: getMarkdownMorTermsOfServiceMd\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mor/privacy-policy/\n  method: get\n  operationId: getPageMorPrivacyPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mor/privacy-policy.md\n  method: get\n  operationId: getMarkdownMorPrivacyPolicyMd\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mor/prohibited-products-and-services/\n  method: get\n  operationId: getPageMorProhibitedProductsAndServices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mor/prohibited-products-and-services.md\n  method: get\n  operationId: getMarkdownMorProhibitedProductsAndServicesMd\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platforms/terms-of-service/\n  method: get\n  operationId: getPagePlatformsTermsOfService\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platforms/terms-of-service.md\n  method: get\n  operationId: getMarkdownPlatformsTermsOfServiceMd\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platforms/merchanting-terms/\n  method: get\n  operationId: getPagePlatformsMerchantingTerms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platforms/merchanting-terms.md\n  method: get\n  operationId: getMarkdownPlatformsMerchantingTermsMd\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platforms/tos-privacy/\n  method: get\n  operationId: getPagePlatformsTosPrivacy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /platforms/tos-privacy.md\n  method: get\n  operationId: getMarkdownPlatformsTosPrivacyMd\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /404.md\n  method: get\n  operationId: getMarkdownNotFound\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/site.json\n  method: get\n  operationId: getSite\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/pages.json\n  method: get\n  operationId: getPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/pricing/mor.json\n  method: get\n  operationId: getMorPricing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/pricing/platforms.json\n\
  \  method: get\n  operationId: getPlatformsPricing\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /openapi.json\n  method: get\n  operationId: getOpenapiJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/openapi.json\n  method: get\n  operationId: getApiOpenapiJson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /skill.md\n  method: get\n  operationId: getSkill\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /llms.txt\n  method: get\n  operationId: getLlmsTxt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/payments-ai/agentic-access/payments-ai-agentic-access.yml
summary_line: 102 operations · 35 acting · 1 human-in-the-loop
tags:
- Company
- Payments
- Artificial Intelligence
- Fintech
- Merchant of Record
- Payment Orchestration
---
