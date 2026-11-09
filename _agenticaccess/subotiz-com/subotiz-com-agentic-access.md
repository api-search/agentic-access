---
acting_count: 44
action_class_counts:
  acting: 44
  connected: 64
api_specs:
- filename: subotiz-com-checkout-session-api-openapi.yml
  format: yaml
  label: subotiz-com Checkout Session API
  slug: subotiz-com-checkout-session-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/subotiz-com/openapi/subotiz-com-checkout-session-api-openapi.yml
- filename: subotiz-com-customer-api-openapi.yml
  format: yaml
  label: subotiz-com Customer API
  slug: subotiz-com-customer-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/subotiz-com/openapi/subotiz-com-customer-api-openapi.yml
- filename: subotiz-com-customer-portal-api-openapi.yml
  format: yaml
  label: subotiz-com Customer Portal API
  slug: subotiz-com-customer-portal-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/subotiz-com/openapi/subotiz-com-customer-portal-api-openapi.yml
- filename: subotiz-com-default-api-openapi.yml
  format: yaml
  label: subotiz-com 争议 API
  slug: subotiz-com-default-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/subotiz-com/openapi/subotiz-com-default-api-openapi.yml
- filename: subotiz-com-discount-api-openapi.yml
  format: yaml
  label: subotiz-com Discount API
  slug: subotiz-com-discount-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/subotiz-com/openapi/subotiz-com-discount-api-openapi.yml
- filename: subotiz-com-invoice-api-openapi.yml
  format: yaml
  label: subotiz-com Invoice API
  slug: subotiz-com-invoice-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/subotiz-com/openapi/subotiz-com-invoice-api-openapi.yml
- filename: subotiz-com-payment-api-openapi.yml
  format: yaml
  label: subotiz-com Payment API
  slug: subotiz-com-payment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/subotiz-com/openapi/subotiz-com-payment-api-openapi.yml
- filename: subotiz-com-price-api-openapi.yml
  format: yaml
  label: subotiz-com Price API
  slug: subotiz-com-price-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/subotiz-com/openapi/subotiz-com-price-api-openapi.yml
- filename: subotiz-com-product-api-openapi.yml
  format: yaml
  label: subotiz-com Product API
  slug: subotiz-com-product-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/subotiz-com/openapi/subotiz-com-product-api-openapi.yml
- filename: subotiz-com-refund-api-openapi.yml
  format: yaml
  label: subotiz-com Refund API
  slug: subotiz-com-refund-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/subotiz-com/openapi/subotiz-com-refund-api-openapi.yml
- filename: subotiz-com-subscription-api-openapi.yml
  format: yaml
  label: subotiz-com Subscription API
  slug: subotiz-com-subscription-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/subotiz-com/openapi/subotiz-com-subscription-api-openapi.yml
- filename: subotiz-com-trade-api-openapi.yml
  format: yaml
  label: subotiz-com Trade API
  slug: subotiz-com-trade-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/subotiz-com/openapi/subotiz-com-trade-api-openapi.yml
- filename: subotiz-com-webhook-api-openapi.yml
  format: yaml
  label: subotiz-com Webhook API
  slug: subotiz-com-webhook-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/subotiz-com/openapi/subotiz-com-webhook-api-openapi.yml
consequence_counts:
  physical: 8
  read: 64
  safety-critical: 4
  write: 32
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 4
kind: agentic-access
layout: agentic-access
method: generated
name: Subotiz Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/subscription/{subscription_id}/revoke-cancel
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/subscription/{subscription_id}/revoke-cancel
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/subscription/{subscription_id}/revoke-price-change
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /api/v1/subscription/{subscription_id}/revoke-price-change
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/session
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/session
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/session/{session_id}/expire
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/session/{session_id}/expire
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/trades
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/trades
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/trades/{trade_id}/refunds
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/trades/{trade_id}/refunds
operation_count: 108
overview: 'subotiz-com exposes 108 API operations that an AI agent could call, of which 44 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 64 read, 32 write, 8 physical, and 4 safety-critical.


  4 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: subotiz-com
provider_slug: subotiz-com
slug: subotiz-com-agentic-access
source_filename: subotiz-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/subotiz-com-openapi.yml, openapi/v1-en.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 108\n  by_action_class:\n    acting: 44\n    connected: 64\n  by_consequence:\n    write: 32\n    read: 64\n    physical: 8\n    safety-critical: 4\n  human_in_the_loop_required: 4\noperations:\n- path: /api/v1/front/customer/create\n  method: post\n  operationId: v1-customer-create-customer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/front/customer/update\n\
  \  method: post\n  operationId: v1-customer-update-customer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/front/customer/{customer_id}\n  method: get\n  operationId: v1-customer-Get-customer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/front/customer\n  method: get\n  operationId: v1-customer-list-customer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/front/customer/delete\n  method: post\n  operationId: v1-customer-delete-customer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customer_portal/auth\n  method: post\n  operationId: v1-customer-portal-api-auth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/discount/{id}\n  method: get\n  operationId: v1-discount-get-discount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/discount\n  method: get\n  operationId: v1-discount-list-discount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /api/v1/discount/{id}/end\n  method: post\n  operationId: v1-discount-end-discount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/disputes\n  method: get\n  operationId: v1-dispute-list-dispute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/disputes/{dispute_id}\n  method: get\n  operationId: v1-dispute-get-dispute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/invoices\n  method: get\n  operationId: v1-invoice-list-invoice\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/invoices/{invoice_id}\n  method: get\n  operationId: v1-invoice-get-invoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/payments\n  method: get\n  operationId: v1-payment-list-payments-by-trade-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/payments/list\n  method: get\n  operationId: v1-payment-query-payments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/prices/{price_id}\n  method: get\n  operationId: v1-price-get-price\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/v1/prices\n  method: get\n  operationId: v1-price-list-price\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/prices\n  method: post\n  operationId: v1-price-create-price\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/prices/version/{price_version_id}\n  method: get\n  operationId: v1-price-get-price-version\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/prices/version\n  method: get\n  operationId: v1-price-list-price-version\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/prices/{price_version_id}/status\n  method: post\n  operationId: v1-price-change-price-status\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/products/{product_id}\n  method: get\n  operationId: v1-product-get-product\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/products\n  method: get\n  operationId: v1-product-list-product\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/products\n  method: post\n\
  \  operationId: v1-product-create-product\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/products/version/{product_version_id}\n  method: get\n  operationId: v1-product-get-product-version\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/products/version\n  method: get\n  operationId: v1-product-list-product-version\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/products/{product_version_id}/status\n  method: post\n  operationId: v1-product-change-product-status\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/product-categories\n  method: get\n  operationId: v1-product-list-product-categories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/trades/{trade_id}/refunds\n  method: get\n  operationId: v1-refund-list-refund\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/trades/{trade_id}/refunds\n  method: post\n  operationId: v1-refund-create-refund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/trades/{trade_id}/refunds/{refund_id}\n  method: get\n  operationId: v1-refund-get-refund\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/session\n  method: get\n  operationId: v1-checkout-session-list-checkout-session\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/session\n  method: post\n  operationId: v1-checkout-session-create-checkout-session\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/session/{session_id}\n  method: get\n  operationId: v1-checkout-session-get-checkout-session\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/session/{session_id}/expire\n  method: post\n  operationId: v1-checkout-session-expire-checkout-session\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/subscription/{subscription_id}\n  method: get\n  operationId: v1-subscription-get-subscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/v1/subscription/{subscription_id}\n  method: post\n  operationId: v1-subscription-update-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/subscription\n  method: get\n  operationId: v1-subscription-list-subscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/subscription/{subscription_id}/cancel\n  method: post\n  operationId: v1-subscription-cancel-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/subscription/{subscription_id}/renewal\n  method: post\n  operationId: v1-subscription-renewal-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/subscription/{subscription_id}/record_usage\n  method: post\n  operationId: v1-subscription-record-subscription-usage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/subscription/{subscription_id}/update/fixed_term\n  method: post\n  operationId: v1-subscription-update-subscription-fixed-term\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/subscription/{subscription_id}/usage\n  method: get\n  operationId: v1-subscription-get-subscription-usage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/subscription/{subscription_id}/pause\n  method: post\n  operationId: v1-subscription-pause-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/subscription/{subscription_id}/resume\n\
  \  method: post\n  operationId: v1-subscription-resume-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/subscription/{subscription_id}/revoke-cancel\n  method: post\n  operationId: v1-subscription-revoke-cancel-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/subscription/{subscription_id}/revoke-price-change\n  method: post\n  operationId: v1-subscription-revoke-price-change\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/subscription/{subscription_id}/quantity-preview\n  method: get\n  operationId: v1-subscription-preview-subscription-quantity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/trades\n  method: get\n  operationId: v1-trade-list-trade\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/trades\n  method: post\n  operationId: v1-trade-create-trade\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/trades/{trade_id}\n  method: get\n  operationId: v1-trade-get-trade\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhook-event\n  method: get\n  operationId: v1-webhook-list-webhook-event\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/webhook/endpoints\n  method: get\n  operationId: v1-webhook-list-endpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/webhook/events\n  method: get\n  operationId: v2-webhook-list-event\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/front/customer/create\n  method: post\n  operationId: v1-customer-create-customer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/front/customer/update\n  method: post\n  operationId: v1-customer-update-customer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/front/customer/{customer_id}\n  method: get\n  operationId: v1-customer-Get-customer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/front/customer\n  method: get\n  operationId: v1-customer-list-customer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/front/customer/delete\n  method: post\n  operationId: v1-customer-delete-customer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/customer_portal/auth\n  method: post\n  operationId: v1-customer-portal-api-auth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/discount/{id}\n  method: get\n  operationId: v1-discount-get-discount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/discount\n  method: get\n  operationId: v1-discount-list-discount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/discount/{id}/end\n  method: post\n  operationId: v1-discount-end-discount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/disputes\n  method: get\n  operationId: v1-dispute-list-dispute\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/disputes/{dispute_id}\n  method: get\n  operationId: v1-dispute-get-dispute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/invoices\n  method: get\n  operationId: v1-invoice-list-invoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/invoices/{invoice_id}\n  method: get\n  operationId: v1-invoice-get-invoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/payments\n  method: get\n  operationId: v1-payment-list-payments-by-trade-id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/payments/list\n  method: get\n  operationId: v1-payment-query-payments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/prices/{price_id}\n  method: get\n  operationId: v1-price-get-price\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/prices\n  method: get\n  operationId: v1-price-list-price\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/prices\n  method: post\n  operationId: v1-price-create-price\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/prices/version/{price_version_id}\n  method: get\n  operationId: v1-price-get-price-version\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/prices/version\n  method: get\n  operationId: v1-price-list-price-version\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/prices/{price_version_id}/status\n  method: post\n  operationId: v1-price-change-price-status\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/products/{product_id}\n\
  \  method: get\n  operationId: v1-product-get-product\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/products\n  method: get\n  operationId: v1-product-list-product\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/products\n  method: post\n  operationId: v1-product-create-product\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/products/version/{product_version_id}\n  method: get\n  operationId: v1-product-get-product-version\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/products/version\n  method: get\n  operationId: v1-product-list-product-version\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/products/{product_version_id}/status\n  method: post\n  operationId: v1-product-change-product-status\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/product-categories\n  method: get\n  operationId: v1-product-list-product-categories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/trades/{trade_id}/refunds\n  method: get\n  operationId:\
  \ v1-refund-list-refund\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/trades/{trade_id}/refunds\n  method: post\n  operationId: v1-refund-create-refund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/trades/{trade_id}/refunds/{refund_id}\n  method: get\n  operationId: v1-refund-get-refund\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/session\n  method: get\n  operationId: v1-checkout-session-list-checkout-session\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/session\n  method: post\n  operationId: v1-checkout-session-create-checkout-session\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/session/{session_id}\n  method: get\n  operationId: v1-checkout-session-get-checkout-session\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/session/{session_id}/expire\n  method: post\n  operationId: v1-checkout-session-expire-checkout-session\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/subscription/{subscription_id}\n  method: get\n  operationId: v1-subscription-get-subscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/subscription/{subscription_id}\n  method: post\n  operationId: v1-subscription-update-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/subscription\n  method: get\n  operationId: v1-subscription-list-subscription\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/subscription/{subscription_id}/cancel\n  method: post\n  operationId: v1-subscription-cancel-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/subscription/{subscription_id}/renewal\n  method: post\n  operationId: v1-subscription-renewal-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/subscription/{subscription_id}/record_usage\n  method: post\n\
  \  operationId: v1-subscription-record-subscription-usage\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/subscription/{subscription_id}/update/fixed_term\n  method: post\n  operationId: v1-subscription-update-subscription-fixed-term\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/subscription/{subscription_id}/usage\n  method: get\n  operationId: v1-subscription-get-subscription-usage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /api/v1/subscription/{subscription_id}/pause\n  method: post\n  operationId: v1-subscription-pause-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/subscription/{subscription_id}/resume\n  method: post\n  operationId: v1-subscription-resume-subscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/subscription/{subscription_id}/revoke-cancel\n  method: post\n  operationId: v1-subscription-revoke-cancel-subscription\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/subscription/{subscription_id}/revoke-price-change\n  method: post\n  operationId: v1-subscription-revoke-price-change\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1/subscription/{subscription_id}/quantity-preview\n  method: get\n  operationId: v1-subscription-preview-subscription-quantity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/v1/trades\n  method: get\n  operationId: v1-trade-list-trade\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/trades\n  method: post\n  operationId: v1-trade-create-trade\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/trades/{trade_id}\n  method: get\n  operationId: v1-trade-get-trade\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/webhook-event\n  method: get\n  operationId: v1-webhook-list-webhook-event\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/webhook/endpoints\n  method: get\n  operationId: v1-webhook-list-endpoint\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/webhook/events\n  method: get\n  operationId: v2-webhook-list-event\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://artifacts.apis.io/subotiz-com/agentic-access/subotiz-com-agentic-access.yml
summary_line: 108 operations · 44 acting · 4 human-in-the-loop
tags:
- Payments
- Artificial Intelligence
- Billing
- Software-as-a-Service
- Fintech
- Company
---
