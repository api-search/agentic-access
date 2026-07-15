---
acting_count: 75
action_class_counts:
  acting: 75
  connected: 36
api_specs:
- filename: paypal-billing-subscriptions-openapi-original.yml
  format: yaml
  label: PayPal Billing Subscriptions API
  slug: paypal-billing-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-billing-subscriptions-openapi-original.yml
- filename: paypal-catalog-products-openapi-original.yml
  format: yaml
  label: PayPal Catalog Products API
  slug: paypal-products-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-catalog-products-openapi-original.yml
- filename: paypal-checkout-orders-openapi-original.yml
  format: yaml
  label: PayPal Orders API
  slug: paypal-orders-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-checkout-orders-openapi-original.yml
- filename: paypal-customer-disputes-openapi-original.yml
  format: yaml
  label: PayPal Customer Disputes API
  slug: paypal-disputes-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-customer-disputes-openapi-original.yml
- filename: paypal-customer-partner-referrals-openapi-original.yml
  format: yaml
  label: PayPal Partner Referrals API
  slug: paypal-partner-referrals-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-customer-partner-referrals-openapi-original.yml
- filename: paypal-invoicing-openapi-original.yml
  format: yaml
  label: PayPal Invoicing API
  slug: paypal-invoicing-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-invoicing-openapi-original.yml
- filename: paypal-notification-webhooks-openapi-original.yml
  format: yaml
  label: PayPal Notification Webhooks API
  slug: paypal-notification-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-notification-webhooks-openapi-original.yml
- filename: paypal-payment-experience-openapi-original.yml
  format: yaml
  label: PayPal Payment Experience API
  slug: paypal-payment-experience-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-payment-experience-openapi-original.yml
- filename: paypal-payments-openapi-original.yml
  format: yaml
  label: PayPal Payments API
  slug: paypal-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-payments-openapi-original.yml
- filename: paypal-payouts-openapi-original.yml
  format: yaml
  label: PayPal Payouts API
  slug: paypal-payouts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-payouts-openapi-original.yml
- filename: paypal-reporting-transactions-openapi-original.yml
  format: yaml
  label: PayPal Transaction Search (Reporting) API
  slug: paypal-reporting-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-reporting-transactions-openapi-original.yml
- filename: paypal-shipping-tracking-openapi-original.yml
  format: yaml
  label: PayPal Shipping Tracking API
  slug: paypal-shipping-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-shipping-tracking-openapi-original.yml
- filename: paypal-vault-payment-tokens-openapi-original.yml
  format: yaml
  label: PayPal Vault Payment Tokens API
  slug: paypal-payment-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/openapi/paypal-vault-payment-tokens-openapi-original.yml
consequence_counts:
  physical: 38
  read: 36
  write: 37
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Paypal Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/billing/subscriptions/{id}/capture
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/customer/disputes/{id}/send-message
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/notifications/webhooks-events/{event_id}/resend
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payment-experience/web-profiles
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/payment-experience/web-profiles/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v1/payment-experience/web-profiles/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/payment-experience/web-profiles/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payments/payouts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payments/payouts-item/{payout_item_id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/shipping/trackers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/shipping/trackers-batch
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/shipping/trackers/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/checkout/orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v2/checkout/orders/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/checkout/orders/{id}/authorize
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/checkout/orders/{id}/capture
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/checkout/orders/{id}/confirm-payment-source
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/checkout/orders/{id}/track
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /v2/checkout/orders/{id}/trackers/{tracker_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/invoicing/generate-next-invoice-number
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/invoicing/invoices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v2/invoicing/invoices/{invoice_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v2/invoicing/invoices/{invoice_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/invoicing/invoices/{invoice_id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/invoicing/invoices/{invoice_id}/generate-qr-code
operation_count: 111
overview: 'PayPal exposes 111 API operations that an AI agent could call, of which 75 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 36 read, 37 write, and 38 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: PayPal
provider_slug: paypal
slug: paypal-agentic-access
source_filename: paypal-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/paypal-billing-subscriptions-openapi-original.yml, openapi/paypal-catalog-products-openapi-original.yml,\n  openapi/paypal-checkout-orders-openapi-original.yml, openapi/paypal-customer-disputes-openapi-original.yml,\n  openapi/paypal-customer-partner-referrals-openapi-original.yml, openapi/paypal-invoicing-openapi-original.yml,\n  openapi/paypal-notification-webhooks-openapi-original.yml, openapi/paypal-payment-experience-openapi-original.yml,\n  openapi/paypal-payments-openapi-original.yml, openapi/paypal-payouts-openapi-original.yml,\n  openapi/paypal-reporting-transactions-openapi-original.yml, openapi/paypal-shipping-tracking-openapi-original.yml,\n  openapi/paypal-vault-payment-tokens-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment.\
  \ See research/curity/agentic-governance/.\nsummary:\n  operations: 111\n  by_action_class:\n    acting: 75\n    connected: 36\n  by_consequence:\n    write: 37\n    read: 36\n    physical: 38\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/billing/plans\n  method: post\n  operationId: plans.create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/subscriptions\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/plans\n  method: get\n  operationId: plans.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://uri.paypal.com/services/subscriptions\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing/plans/{id}\n  method: get\n  operationId: plans.get\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://uri.paypal.com/services/subscriptions\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing/plans/{id}\n  method: patch\n  operationId: plans.patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/subscriptions\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/plans/{id}/activate\n  method: post\n  operationId: plans.activate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/subscriptions\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/plans/{id}/deactivate\n  method: post\n  operationId: plans.deactivate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/subscriptions\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/plans/{id}/update-pricing-schemes\n  method: post\n  operationId: plans.update-pricing-schemes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/subscriptions\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/subscriptions\n  method: post\n\
  \  operationId: subscriptions.create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/subscriptions\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/subscriptions/{id}\n  method: get\n  operationId: subscriptions.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://uri.paypal.com/services/subscriptions\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/billing/subscriptions/{id}\n  method: patch\n  operationId: subscriptions.patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/subscriptions\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/subscriptions/{id}/revise\n  method: post\n  operationId: subscriptions.revise\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/subscriptions\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/subscriptions/{id}/suspend\n  method: post\n  operationId: subscriptions.suspend\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/subscriptions\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/billing/subscriptions/{id}/cancel\n  method: post\n  operationId: subscriptions.cancel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/subscriptions\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/subscriptions/{id}/activate\n  method: post\n  operationId: subscriptions.activate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/subscriptions\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/subscriptions/{id}/capture\n  method: post\n  operationId: subscriptions.capture\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/subscriptions\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/subscriptions/{id}/transactions\n  method: get\n  operationId: subscriptions.transactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://uri.paypal.com/services/subscriptions\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/catalogs/products\n  method: post\n  operationId: products.create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/subscriptions\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/catalogs/products\n  method: get\n  operationId: products.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://uri.paypal.com/services/subscriptions\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/catalogs/products/{product_id}\n  method: get\n  operationId: products.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://uri.paypal.com/services/subscriptions\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/catalogs/products/{product_id}\n  method: patch\n  operationId: products.patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/subscriptions\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/checkout/orders\n  method: post\n  operationId: orders.create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/payments/orders/client-side-integration\n    - https://uri.paypal.com/services/payments/payment\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/checkout/orders/{id}\n  method: get\n  operationId: orders.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://uri.paypal.com/services/payments/orders/client-side-integration\n    - https://uri.paypal.com/services/payments/payment\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/checkout/orders/{id}\n  method: patch\n  operationId: orders.patch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/payments/orders/client-side-integration\n    - https://uri.paypal.com/services/payments/payment\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/checkout/orders/{id}/confirm-payment-source\n  method: post\n  operationId: orders.confirm\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/payments/initiatepayment\n    - https://uri.paypal.com/services/payments/payment\n    audience: null\n    token:\n      max-ttl: 300\n    \
  \  exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/checkout/orders/{id}/authorize\n  method: post\n  operationId: orders.authorize\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/payments/orders/client-side-integration\n    - https://uri.paypal.com/services/payments/payment\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/checkout/orders/{id}/capture\n  method: post\n  operationId: orders.capture\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/payments/orders/client-side-integration\n\
  \    - https://uri.paypal.com/services/payments/payment\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/checkout/orders/{id}/track\n  method: post\n  operationId: orders.track.create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/payments/payment\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/checkout/orders/{id}/trackers/{tracker_id}\n  method: patch\n  operationId: orders.trackers.patch\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n\
  \    - https://uri.paypal.com/services/payments/payment\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customer/disputes\n  method: get\n  operationId: disputes.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://uri.paypal.com/services/disputes/read\n    - https://uri.paypal.com/services/disputes/read-buyer\n    - https://uri.paypal.com/services/disputes/read-ebay\n    - https://uri.paypal.com/services/disputes/read-partner\n    - https://uri.paypal.com/services/disputes/read-seller\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customer/disputes/{id}\n  method: get\n  operationId: disputes.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n\
  \    - https://uri.paypal.com/services/disputes/read\n    - https://uri.paypal.com/services/disputes/read-buyer\n    - https://uri.paypal.com/services/disputes/read-ebay\n    - https://uri.paypal.com/services/disputes/read-partner\n    - https://uri.paypal.com/services/disputes/read-seller\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customer/disputes/{id}\n  method: patch\n  operationId: disputes.patch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/disputes/update-seller\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customer/disputes/{id}/provide-evidence\n  method: post\n  operationId: disputes.provide-evidence\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    -\
  \ https://uri.paypal.com/services/disputes/update-buyer\n    - https://uri.paypal.com/services/disputes/update-partner\n    - https://uri.paypal.com/services/disputes/update-seller\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customer/disputes/{id}/appeal\n  method: post\n  operationId: disputes.appeal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/disputes/update-buyer\n    - https://uri.paypal.com/services/disputes/update-seller\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customer/disputes/{id}/accept-claim\n  method: post\n  operationId: disputes.accept-claim\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/disputes/update-seller\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customer/disputes/{id}/adjudicate\n  method: post\n  operationId: disputes.adjudicate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/disputes/update-buyer\n    - https://uri.paypal.com/services/disputes/update-seller\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customer/disputes/{id}/require-evidence\n  method: post\n  operationId: disputes.require-evidence\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/disputes/update-buyer\n    - https://uri.paypal.com/services/disputes/update-seller\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customer/disputes/{id}/escalate\n  method: post\n  operationId: disputes.escalate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/disputes/update-buyer\n    - https://uri.paypal.com/services/disputes/update-seller\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customer/disputes/{id}/send-message\n  method: post\n  operationId: disputes.send-message\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: physical\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/disputes/update-buyer\n    - https://uri.paypal.com/services/disputes/update-seller\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customer/disputes/{id}/make-offer\n  method: post\n  operationId: disputes.make-offer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/disputes/update-buyer\n    - https://uri.paypal.com/services/disputes/update-seller\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customer/disputes/{id}/accept-offer\n  method: post\n  operationId:\
  \ disputes.accept-offer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/disputes/update-buyer\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customer/disputes/{id}/deny-offer\n  method: post\n  operationId: disputes.deny-offer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/disputes/update-buyer\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customer/disputes/{id}/acknowledge-return-item\n  method: post\n  operationId: disputes.acknowledge-return-item\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: write\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/disputes/update-seller\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customer/disputes/{id}/provide-supporting-info\n  method: post\n  operationId: disputes.provide-supporting-info\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/disputes/update-buyer\n    - https://uri.paypal.com/services/disputes/update-partner\n    - https://uri.paypal.com/services/disputes/update-seller\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/customer/partner-referrals\n  method: post\n  operationId: partner-referrals.create\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/customer/partner-referrals/readwrite\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/customer/partner-referrals/{partner_referral_id}\n  method: get\n  operationId: partner-referrals.read\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://uri.paypal.com/services/customer/partner-referrals\n    - https://uri.paypal.com/services/customer/partner-referrals/readwrite\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/invoicing/invoices\n  method: post\n  operationId: invoices.create\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/invoicing/invoices/readwrite\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/invoicing/invoices\n  method: get\n  operationId: invoices.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://uri.paypal.com/services/invoicing/invoices/read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/invoicing/invoices/{invoice_id}/send\n  method: post\n  operationId: invoices.send\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/invoicing/invoices/readwrite\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v2/invoicing/invoices/{invoice_id}/remind\n  method: post\n  operationId: invoices.remind\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/invoicing/invoices/readwrite\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/invoicing/invoices/{invoice_id}/cancel\n  method: post\n  operationId: invoices.cancel\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/invoicing/invoices/readwrite\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v2/invoicing/invoices/{invoice_id}/payments\n  method: post\n  operationId: invoices.payments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/invoicing/invoices/readwrite\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/invoicing/invoices/{invoice_id}/payments/{transaction_id}\n  method: delete\n  operationId: invoices.payments-delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/invoicing/invoices/readwrite\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/invoicing/invoices/{invoice_id}/refunds\n  method: post\n  operationId: invoices.refunds\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/invoicing/invoices/readwrite\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/invoicing/invoices/{invoice_id}/refunds/{transaction_id}\n  method: delete\n  operationId: invoices.refunds-delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/invoicing/invoices/readwrite\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/invoicing/invoices/{invoice_id}/generate-qr-code\n  method: post\n  operationId: invoices.generate-qr-code\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/invoicing/invoices/readwrite\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/invoicing/generate-next-invoice-number\n  method: post\n  operationId: invoicing.generate-next-invoice-number\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/invoicing/invoices/readwrite\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/invoicing/invoices/{invoice_id}\n  method: get\n  operationId: invoices.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://uri.paypal.com/services/invoicing/invoices/read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/invoicing/invoices/{invoice_id}\n  method: put\n  operationId: invoices.update\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/invoicing/invoices/readwrite\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v2/invoicing/invoices/{invoice_id}\n  method: delete\n  operationId: invoices.delete\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/invoicing/invoices/readwrite\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/invoicing/search-invoices\n  method: post\n  operationId: invoices.search-invoices\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/invoicing/invoices/read\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /v2/invoicing/templates\n  method: get\n  operationId: templates.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://uri.paypal.com/services/invoicing/invoices/read\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/invoicing/templates\n  method: post\n  operationId: templates.create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/invoicing/invoices/readwrite\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/invoicing/templates/{template_id}\n  method: get\n  operationId: templates.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://uri.paypal.com/services/invoicing/invoices/read\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/invoicing/templates/{template_id}\n  method: put\n  operationId: templates.update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/invoicing/invoices/readwrite\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/invoicing/templates/{template_id}\n  method: delete\n  operationId: templates.delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/invoicing/invoices/readwrite\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/notifications/webhooks\n  method:\
  \ post\n  operationId: webhooks.post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/applications/webhooks\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/notifications/webhooks\n  method: get\n  operationId: webhooks.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://uri.paypal.com/services/applications/webhooks\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/notifications/webhooks/{webhook_id}\n  method: get\n  operationId: webhooks.get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://uri.paypal.com/services/applications/webhooks\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/notifications/webhooks/{webhook_id}\n  method: patch\n  operationId: webhooks.update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/applications/webhooks\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/notifications/webhooks/{webhook_id}\n  method: delete\n  operationId: webhooks.delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/applications/webhooks\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/notifications/webhooks/{webhook_id}/event-types\n  method: get\n  operationId: event-types.list\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - https://uri.paypal.com/services/applications/webhooks\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/notifications/webhooks-lookup\n  method: post\n  operationId: webhooks-lookup.post\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - https://uri.paypal.com/services/applications/webhooks\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/notifications/webhooks-lookup\n  method: get\n  operationId: webhooks-lookup.list\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope\n\n# --- truncated at 32 KB (47 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/agentic-access/paypal-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paypal/refs/heads/main/agentic-access/paypal-agentic-access.yml
summary_line: 111 operations · 75 acting
tags:
- Billing
- Commerce
- Disputes
- Invoices
- Orders
- Payments
- Payouts
- Subscriptions
- Tokens
- Webhooks
---
