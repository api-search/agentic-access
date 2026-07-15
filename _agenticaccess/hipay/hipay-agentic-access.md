---
acting_count: 23
action_class_counts:
  acting: 23
  connected: 32
api_specs:
- filename: api-gateway.yml
  format: yaml
  label: HiPay Payment Gateway API
  slug: hipay-payment-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/hipay/openapi-hipay/master/enterprise/api-gateway.yml
- filename: gateway.yaml
  format: yaml
  label: HiPay Enterprise Gateway API
  slug: hipay-enterprise-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/hipay/openapi-hipay/master/enterprise/gateway.yaml
- filename: hpayment.yaml
  format: yaml
  label: HiPay Enterprise HostedPage API
  slug: hipay-enterprise-hostedpage-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/hipay/openapi-hipay/master/enterprise/hpayment.yaml
- filename: settlement.yaml
  format: yaml
  label: HiPay Enterprise Finance API
  slug: hipay-enterprise-finance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/hipay/openapi-hipay/master/enterprise/settlement.yaml
- filename: tokenization.yaml
  format: yaml
  label: HiPay Enterprise Tokenization API
  slug: hipay-enterprise-tokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/hipay/openapi-hipay/master/enterprise/tokenization.yaml
- filename: applepay-web.yaml
  format: yaml
  label: HiPay Apple Pay Web API
  slug: hipay-apple-pay-web-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/hipay/openapi-hipay/master/enterprise/applepay-web.yaml
- filename: pos_api.yaml
  format: yaml
  label: HiPay POS API
  slug: hipay-pos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/hipay/openapi-hipay/master/omnichannel/pos_api.yaml
- filename: omnichannel.yaml
  format: yaml
  label: HiPay Omnichannel Gateway API
  slug: hipay-omnichannel-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/hipay/openapi-hipay/master/omnichannel/omnichannel.yaml
- filename: marketplace.yaml
  format: yaml
  label: HiPay Marketplace API
  slug: hipay-marketplace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/hipay/openapi-hipay/master/marketplace/marketplace.yaml
consequence_counts:
  physical: 7
  read: 32
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Hipay Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transfer.{_format}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/applepay/paymentSession
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/connector/order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/hpayment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/order
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /withdrawal.{_format}
operation_count: 55
overview: 'HiPay exposes 55 API operations that an AI agent could call, of which 23 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 32 read, 16 write, and 7 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: HiPay
provider_slug: hipay
slug: hipay-agentic-access
source_filename: hipay-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/api-gateway.yml, openapi/applepay-web.yaml, openapi/gateway.yaml, openapi/hpayment.yaml,\n  openapi/marketplace.yaml, openapi/omnichannel.yaml, openapi/pos-api.yaml, openapi/settlement.yaml,\n  openapi/tokenization.yaml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 55\n  by_action_class:\n    connected: 32\n    acting: 23\n  by_consequence:\n    read: 32\n    physical: 7\n    write: 16\n  human_in_the_loop_required: 0\noperations:\n- path: /v3/order/{orderid}\n  method: get\n  operationId: get_api_order_consultation_public\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/routes/available-payment-products\n\
  \  method: get\n  operationId: get_api_routing_available_payment_products_public\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/transaction/{transaction_reference}\n  method: get\n  operationId: get_api_transaction_consultation_public\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/transactions/{type}/{value}\n  method: get\n  operationId: get_api_transaction_consultations_by_type_public\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/applepay/paymentSession\n  method: post\n  operationId: createPaymentSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n\
  \      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/maintenance/transaction/{transaction_reference}\n  method: post\n  operationId: performMaintenanceOperation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/order\n  method: post\n  operationId: requestNewOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transaction/{transaction_reference}\n\
  \  method: get\n  operationId: getTransactionByReference\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transaction\n  method: get\n  operationId: getTransactionsByReference\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/hpayment\n  method: post\n  operationId: generatePage\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user-account.{_format}\n  method: get\n  operationId: get_user-account\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /user-account.{_format}\n  method: patch\n  operationId: patch_User-account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user-account.{_format}\n  method: post\n  operationId: post_user-account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user-account/sub-account.{_format}\n  method: post\n  operationId: post_user-account_sub-account\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user-account/is-available.{_format}\n  method: post\n  operationId: post_user-account_is-available\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identification.{_format}\n  method: get\n  operationId: get_Identification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /identification.{_format}\n  method: post\n  operationId: post_Identification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ubo.{_format}\n  method: post\n  operationId: post_Ubo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ubo/{id}.{_format}\n  method: delete\n  operationId: delete_ubo\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ubo/legal-representative.{_format}\n  method: post\n  operationId: post_Ubo-legal-representative\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ubo/ubo-statement.{_format}\n  method: delete\n  operationId: delete_ubo-statement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ubo/ubo-statement.{_format}\n  method: get\n  operationId: get_ubo-statement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ubo/ubo-statement.{_format}\n  method: post\n  operationId: post_ubo-statement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user-account/bank-info.{_format}\n  method: post\n  operationId: post_user-account_bank-info\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /user-account/bank-info/{locale}.{_format}\n  method: get\n  operationId: get_user-account_bank-info_locale\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /user-account/balance.{_format}\n  method: get\n  operationId: get_user-account_balance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /transfer.{_format}\n  method: post\n  operationId: post_transfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /withdrawal.{_format}\n  method: post\n  operationId: post_withdrawal\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction.{_format}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction/{id}.{_format}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchant-group/{merchant_group_code}.{_format}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /merchant-group/{merchant_group_code}/count.{_format}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /marketplace/invoice.{_format}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /marketplace/invoice/{reference}.{_format}\n  method: get\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tools/captcha.{_format}\n  method: get\n  operationId: get_Captcha-generation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tools/bank-info-fields/{country}/{locale}.{_format}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tools/business-lines/{locale}.{_format}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tools/locale/codes.{_format}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tools/locale/countries/{locale}.{_format}\n\
  \  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tools/locale/currencies/{locale}.{_format}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tools/locale/timezones.{_format}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tools/website-topics/{business_line_id}/{locale}.{_format}\n  method: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/order\n  method: post\n  operationId: requestNewOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/maintenance/transaction/{transaction_reference}\n  method: post\n  operationId: performMaintenanceOperation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transaction\n  method: get\n  operationId: getOrderTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transaction/{transaction_reference}\n  method: get\n  operationId: getTransactionDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/connector/order\n  method: post\n  operationId: postOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/connector/healthcheck\n  method: get\n  operationId: healthcheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /settlement\n  method: get\n  operationId: getSettlements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /settlement/{id}\n  method: get\n  operationId: getSettlementItem\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /settlement/{id}/raw{ext}\n  method: get\n  operationId: getSettlementRaw\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /create\n  method: post\n  operationId: createToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{token}\n  method: get\n  operationId: lookupToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /\n  method: delete\n  operationId: deleteToken\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /update\n  method: post\n  operationId: updateToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/hipay/refs/heads/main/agentic-access/hipay-agentic-access.yml
summary_line: 55 operations · 23 acting
tags:
- Payments
- Fintech
- Europe
- Omnichannel
- Point of Sale
- Fraud Prevention
- Tokenization
- Marketplace
---
