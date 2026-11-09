---
acting_count: 28
action_class_counts:
  acting: 28
  connected: 30
api_specs:
- filename: breezecash-customers-api-openapi.yml
  format: yaml
  label: Breeze.cash Customers API
  slug: breezecash-customers-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breezecash/openapi/breezecash-customers-api-openapi.yml
- filename: breezecash-direct-payment-api-openapi.yml
  format: yaml
  label: Breeze.cash Direct Payment API
  slug: breezecash-direct-payment-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breezecash/openapi/breezecash-direct-payment-api-openapi.yml
- filename: breezecash-disputes-api-openapi.yml
  format: yaml
  label: Breeze.cash Disputes API
  slug: breezecash-disputes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breezecash/openapi/breezecash-disputes-api-openapi.yml
- filename: breezecash-fraud-reports-api-openapi.yml
  format: yaml
  label: Breeze.cash Fraud Reports API
  slug: breezecash-fraud-reports-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breezecash/openapi/breezecash-fraud-reports-api-openapi.yml
- filename: breezecash-headless-kyc-api-openapi.yml
  format: yaml
  label: Breeze.cash Headless KYC API
  slug: breezecash-headless-kyc-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breezecash/openapi/breezecash-headless-kyc-api-openapi.yml
- filename: breezecash-headless-payout-api-openapi.yml
  format: yaml
  label: Breeze.cash Headless Payout API
  slug: breezecash-headless-payout-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breezecash/openapi/breezecash-headless-payout-api-openapi.yml
- filename: breezecash-invoices-api-openapi.yml
  format: yaml
  label: Breeze.cash Invoices API
  slug: breezecash-invoices-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breezecash/openapi/breezecash-invoices-api-openapi.yml
- filename: breezecash-liquidation-addresses-api-openapi.yml
  format: yaml
  label: Breeze.cash Liquidation Addresses API
  slug: breezecash-liquidation-addresses-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breezecash/openapi/breezecash-liquidation-addresses-api-openapi.yml
- filename: breezecash-offramp-api-openapi.yml
  format: yaml
  label: Breeze.cash Offramp API
  slug: breezecash-offramp-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breezecash/openapi/breezecash-offramp-api-openapi.yml
- filename: breezecash-payment-pages-api-openapi.yml
  format: yaml
  label: Breeze.cash Payment Pages API
  slug: breezecash-payment-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breezecash/openapi/breezecash-payment-pages-api-openapi.yml
- filename: breezecash-payout-pages-api-openapi.yml
  format: yaml
  label: Breeze.cash Payout Pages API
  slug: breezecash-payout-pages-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breezecash/openapi/breezecash-payout-pages-api-openapi.yml
- filename: breezecash-products-api-openapi.yml
  format: yaml
  label: Breeze.cash Products API
  slug: breezecash-products-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breezecash/openapi/breezecash-products-api-openapi.yml
- filename: breezecash-risk-api-openapi.yml
  format: yaml
  label: Breeze.cash Risk API
  slug: breezecash-risk-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breezecash/openapi/breezecash-risk-api-openapi.yml
- filename: breezecash-statements-api-openapi.yml
  format: yaml
  label: Breeze.cash Statements API
  slug: breezecash-statements-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breezecash/openapi/breezecash-statements-api-openapi.yml
- filename: breezecash-subscriptions-api-openapi.yml
  format: yaml
  label: Breeze.cash Subscriptions API
  slug: breezecash-subscriptions-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breezecash/openapi/breezecash-subscriptions-api-openapi.yml
- filename: breezecash-tax-api-openapi.yml
  format: yaml
  label: Breeze.cash Tax API
  slug: breezecash-tax-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breezecash/openapi/breezecash-tax-api-openapi.yml
- filename: breezecash-webhooks-api-openapi.yml
  format: yaml
  label: Breeze.cash Webhooks API
  slug: breezecash-webhooks-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/breezecash/openapi/breezecash-webhooks-api-openapi.yml
consequence_counts:
  physical: 12
  read: 30
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Breezecash Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/gateway/customers/{customerId}/payment-methods/{savedPaymentMethodId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/gateway/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/gateway/payments/{pageId}/authentications
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/headless_payout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payment_pages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payment_pages/{pageId}/expire
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payment_pages/{pageId}/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payout_pages
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payout_pages/{id}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payout_pages/{id}/release
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payout_pages/{id}/sandbox_confirm
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/sandbox/disputes
operation_count: 58
overview: 'Breeze.cash exposes 58 API operations that an AI agent could call, of which 28 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 30 read, 16 write, and 12 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Breeze.cash
provider_slug: breezecash
slug: breezecash-agentic-access
source_filename: breezecash-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-29'\nmethod: generated\nsource: openapi/breezecash-breeze-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 58\n  by_action_class:\n    acting: 28\n    connected: 30\n  by_consequence:\n    write: 16\n    read: 30\n    physical: 12\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/customers\n  method: post\n  operationId: createCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customers\n  method: get\n  operationId: getCustomerByQuery\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customers/{id}\n  method: get\n  operationId: getCustomerById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customers/{id}\n  method: post\n  operationId: updateCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customers/{id}/offboard\n  method: post\n  operationId: offboardCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /v1/disputes\n  method: get\n  operationId: listDisputes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fraud_reports\n  method: get\n  operationId: listFraudReports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/fraud_reports/{fraudReportId}\n  method: get\n  operationId: getFraudReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/gateway/customers/{customerId}/payment-methods\n  method: get\n  operationId: listGatewayCustomerPaymentMethods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/gateway/customers/{customerId}/payment-methods/{savedPaymentMethodId}\n  method: delete\n  operationId: deleteGatewayCustomerPaymentMethod\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/gateway/payments\n  method: post\n  operationId: createGatewayPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/gateway/payments/{pageId}\n  method: get\n  operationId: getGatewayPayment\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/gateway/payments/{pageId}/authentications\n  method: post\n  operationId: resumeGatewayPaymentAuthentication\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/headless_kyc\n  method: get\n  operationId: getHeadlessKycByCustomerReferenceId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/headless_kyc\n  method: post\n  operationId: submitHeadlessKycWithImageUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/headless_kyc/proof_of_address\n  method: post\n  operationId: submitHeadlessKycProofOfAddressWithUrl\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/headless_kyc/proof_of_address/upload\n  method: post\n  operationId: submitHeadlessKycProofOfAddressWithUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/headless_kyc/{id}\n\
  \  method: get\n  operationId: getHeadlessKycById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/headless_kyc/{id}/initiate_tier_3_kyc\n  method: post\n  operationId: initiateHeadlessKycTier3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/headless_kyc?\n  method: post\n  operationId: submitHeadlessKycWithImageUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/headless_payout\n  method: post\n  operationId:\
  \ createHeadlessPayout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/invoices/{invoiceId}\n  method: get\n  operationId: getInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/liquidation_addresses\n  method: post\n  operationId: createLiquidationAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/liquidation_addresses\n  method: get\n  operationId:\
  \ listLiquidationAddresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/liquidation_addresses/{id}\n  method: get\n  operationId: getLiquidationAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/liquidation_addresses/{id}/transactions\n  method: get\n  operationId: listLiquidationAddressTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/liquidation_addresses/{id}/transactions/{txId}\n  method: get\n  operationId: getLiquidationAddressTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/offramp\n  method: post\n  operationId:\
  \ createOfframpRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/offramp/{id}\n  method: get\n  operationId: getOfframpRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/offramp/{id}/cancel\n  method: post\n  operationId: cancelOfframpRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/offramp/{id}/release\n  method: post\n  operationId: releaseOfframpRequest\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/payment_pages\n  method: post\n  operationId: createPaymentPage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/payment_pages\n  method: get\n  operationId: listPaymentPages\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payment_pages/{pageId}\n  method: get\n  operationId: getPaymentPage\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payment_pages/{pageId}/expire\n  method: post\n  operationId: expirePaymentPage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/payment_pages/{pageId}/payment_details\n  method: get\n  operationId: getAllPaymentAttempts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payment_pages/{pageId}/refund\n  method: post\n  operationId: initiateRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/payment_pages/{pageId}/refund/{refundId}\n  method: get\n  operationId: getRefund\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payout_pages\n  method: post\n  operationId: createPayoutPage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/payout_pages\n  method: get\n  operationId: getPayoutPageHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payout_pages/{id}\n  method: get\n  operationId: getPayoutPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payout_pages/{id}/cancel\n  method: post\n  operationId: cancelPayoutPage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/payout_pages/{id}/release\n  method: post\n  operationId: releasePayoutPage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/payout_pages/{id}/sandbox_confirm\n  method: post\n  operationId: sandboxConfirmPayoutPage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/reports/statements\n  method: get\n  operationId: listStatements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reports/statements/{id}/download\n  method: get\n  operationId: downloadStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /v1/risk\n  method: get\n  operationId: getRiskStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/sandbox/disputes\n  method: post\n  operationId: simulateSandboxDispute\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/subscriptions\n  method: post\n  operationId: createSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v1/subscriptions\n  method: get\n  operationId: listSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/subscriptions/client-reference/{clientReferenceId}\n  method: get\n  operationId: getSubscriptionByClientReferenceId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/subscriptions/{subscriptionId}\n  method: get\n  operationId: getSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/subscriptions/{subscriptionId}/cancel\n  method: post\n  operationId: cancelSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/tax/tax_rate\n  method: get\n  operationId: getMerchantTaxRate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/products\n  method: post\n  operationId: createProduct\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/products\n  method: get\n  operationId: listProducts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/products/{productId}\n  method: get\n  operationId: getProduct\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/products/{productId}/price\n  method: post\n  operationId: createProductPrice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/breezecash/agentic-access/breezecash-agentic-access.yml
summary_line: 58 operations · 28 acting
tags:
- Company
- Fintech
- Payments
- Cryptocurrency
- Startups
---
