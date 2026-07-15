---
acting_count: 31
action_class_counts:
  acting: 31
  connected: 24
api_specs:
- filename: interswitch-web-checkout-api-openapi.yml
  format: yaml
  label: Interswitch Web Checkout API
  slug: interswitch-web-checkout-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interswitch/refs/heads/main/openapi/interswitch-web-checkout-api-openapi.yml
- filename: interswitch-payment-gateway-api-openapi.yml
  format: yaml
  label: Interswitch Payment Gateway API
  slug: interswitch-payment-gateway-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interswitch/refs/heads/main/openapi/interswitch-payment-gateway-api-openapi.yml
- filename: interswitch-transfers-api-openapi.yml
  format: yaml
  label: Interswitch Transfers API
  slug: interswitch-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interswitch/refs/heads/main/openapi/interswitch-transfers-api-openapi.yml
- filename: interswitch-bills-payment-api-openapi.yml
  format: yaml
  label: Interswitch Bills Payment API
  slug: interswitch-bills-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interswitch/refs/heads/main/openapi/interswitch-bills-payment-api-openapi.yml
- filename: interswitch-airtime-recharge-api-openapi.yml
  format: yaml
  label: Interswitch Airtime Recharge API
  slug: interswitch-airtime-recharge-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interswitch/refs/heads/main/openapi/interswitch-airtime-recharge-api-openapi.yml
- filename: interswitch-paycode-api-openapi.yml
  format: yaml
  label: Interswitch Paycode API
  slug: interswitch-paycode-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interswitch/refs/heads/main/openapi/interswitch-paycode-api-openapi.yml
- filename: interswitch-refunds-api-openapi.yml
  format: yaml
  label: Interswitch Refunds API
  slug: interswitch-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interswitch/refs/heads/main/openapi/interswitch-refunds-api-openapi.yml
- filename: interswitch-recurring-payments-api-openapi.yml
  format: yaml
  label: Interswitch Recurring Payments API
  slug: interswitch-recurring-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interswitch/refs/heads/main/openapi/interswitch-recurring-payments-api-openapi.yml
- filename: interswitch-card-360-api-openapi.yml
  format: yaml
  label: Interswitch Card 360 API
  slug: interswitch-card-360-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interswitch/refs/heads/main/openapi/interswitch-card-360-api-openapi.yml
- filename: interswitch-lending-api-openapi.yml
  format: yaml
  label: Interswitch Lending API
  slug: interswitch-lending-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interswitch/refs/heads/main/openapi/interswitch-lending-api-openapi.yml
- filename: interswitch-customer-insights-api-openapi.yml
  format: yaml
  label: Interswitch Customer Insights API
  slug: interswitch-customer-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interswitch/refs/heads/main/openapi/interswitch-customer-insights-api-openapi.yml
- filename: interswitch-transaction-search-api-openapi.yml
  format: yaml
  label: Interswitch Transaction Search API
  slug: interswitch-transaction-search-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/interswitch/refs/heads/main/openapi/interswitch-transaction-search-api-openapi.yml
consequence_counts:
  physical: 16
  read: 24
  safety-critical: 1
  write: 14
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Interswitch Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /card-360/api/v1/cards/{cardId}/pin
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/purchases/recurrents
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/purchases/validations/recurrents
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/quickteller/payments/advices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/quickteller/payments/advices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/quickteller/payments/advices/epin
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /collections/w/pay
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /lending-service/api/v1/loans/{loanId}/debit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /lending-service/api/v2/payments/token
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /lending-service/api/v2/payments/token/validate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paymentgateway/api/v1/hosted-fields/sessions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paymentgateway/api/v1/payment-links
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paymentgateway/api/v1/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paymentgateway/api/v1/refunds
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paymentgateway/api/v1/three-d-secure/sessions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /quicktellerservice/api/v5/transactions/BulkTransfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /quicktellerservice/api/v5/transactions/TransferFunds
operation_count: 55
overview: 'Interswitch exposes 55 API operations that an AI agent could call, of which 31 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 24 read, 14 write, 16 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Interswitch
provider_slug: interswitch
slug: interswitch-agentic-access
source_filename: interswitch-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/interswitch-airtime-recharge-api-openapi.yml, openapi/interswitch-bills-payment-api-openapi.yml,\n  openapi/interswitch-card-360-api-openapi.yml, openapi/interswitch-customer-insights-api-openapi.yml,\n  openapi/interswitch-lending-api-openapi.yml, openapi/interswitch-paycode-api-openapi.yml,\n  openapi/interswitch-payment-gateway-api-openapi.yml, openapi/interswitch-recurring-payments-api-openapi.yml,\n  openapi/interswitch-refunds-api-openapi.yml, openapi/interswitch-transaction-search-api-openapi.yml,\n  openapi/interswitch-transfers-api-openapi.yml, openapi/interswitch-web-checkout-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 55\n  by_action_class:\n    connected:\
  \ 24\n    acting: 31\n  by_consequence:\n    read: 24\n    physical: 16\n    write: 14\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /api/v2/quickteller/categorys/4/billers\n  method: get\n  operationId: listAirtimeTelcos\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/quickteller/billers/{billerId}/paymentitems\n  method: get\n  operationId: listAirtimeDenominations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/quickteller/payments/advices\n  method: post\n  operationId: rechargeAirtime\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/quickteller/payments/advices/epin\n  method: post\n  operationId: purchaseEpinVoucher\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/quickteller/categorys\n  method: get\n  operationId: listBillerCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/quickteller/categorys/{categoryId}/billers\n  method: get\n  operationId: listBillersInCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /api/v2/quickteller/billers\n  method: get\n  operationId: listBillers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/quickteller/billers/{billerId}/paymentitems\n  method: get\n  operationId: listBillerPaymentItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/quickteller/customers/validations\n  method: post\n  operationId: validateCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/quickteller/payments/advices\n  method: post\n  operationId: submitBillPaymentAdvice\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /card-360/api/v1/cards\n  method: post\n  operationId: createCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /card-360/api/v1/cards/{cardId}\n  method: get\n  operationId: getCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /card-360/api/v1/cards/{cardId}/block\n  method: post\n  operationId: blockCard\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /card-360/api/v1/cards/{cardId}/unblock\n  method: post\n  operationId: unblockCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /card-360/api/v1/cards/{cardId}/pin\n  method: post\n  operationId: setCardPin\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n\
  \    audit: required\n- path: /card-360/api/v1/cards/{cardId}/balance\n  method: get\n  operationId: getCardBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /card-360/api/v1/cards/link\n  method: post\n  operationId: linkCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /card-360/api/v1/cards/validate\n  method: post\n  operationId: validateCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /insights/api/v1/customers/{customerId}/demography\n\
  \  method: get\n  operationId: getCustomerDemography\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/api/v1/customers/{customerId}/financial-history\n  method: get\n  operationId: getFinancialHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/api/v1/customers/{customerId}/financial-history/average\n  method: get\n  operationId: getAverageFinancialHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/api/v1/customers/{customerId}/financial-habits\n  method: get\n  operationId: getFinancialHabits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /lending-service/api/v1/offers/providers\n  method: get\n  operationId: listLoanProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lending-service/api/v3/offers\n  method: get\n  operationId: listLoanOffers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lending-service/api/v1/offers/{offerId}/accept\n  method: post\n  operationId: acceptLoanOffer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lending-service/api/v1/loans/{loanId}/fund\n  method: post\n  operationId: fundLoan\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lending-service/api/v1/loans/{loanId}/debit\n  method: post\n  operationId: debitLoanRepayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /lending-service/api/v1/loans/{loanId}/update\n  method: put\n  operationId: updateLoanStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /lending-service/api/v1/users/{customerId}/status\n  method: get\n  operationId: getCustomerLoanStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lending-service/api/v1/users/{customerId}/payment-methods\n  method: get\n  operationId: listCustomerPaymentMethods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /lending-service/api/v2/payments/token\n  method: post\n  operationId: generateLendingPaymentToken\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /lending-service/api/v2/payments/token/validate\n  method: post\n  operationId: validateLendingPaymentTokenOtp\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/pwm/subscribers/{subscriberId}/tokens\n  method: post\n  operationId: generatePaycodeToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/pwm/subscribers/{subscriberId}/tokens/status\n  method: get\n  operationId: getPaycodeTokenStatus\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cardless-service/api/v1/cardless-services/cancel-token\n  method: post\n  operationId: cancelPaycodeToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/pwm/subscribers/{subscriberId}/tokens/bulk\n  method: post\n  operationId: generateBulkPaycodeTokens\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paymentgateway/api/v1/payments\n  method: post\n  operationId: createCardPayment\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paymentgateway/api/v1/payments/{paymentId}\n  method: get\n  operationId: getPayment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paymentgateway/api/v1/hosted-fields/sessions\n  method: post\n  operationId: createHostedFieldsSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /paymentgateway/api/v1/three-d-secure/sessions\n  method: post\n  operationId: createThreeDSecureSession\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paymentgateway/api/v1/payment-links\n  method: post\n  operationId: createPaymentLink\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/purchases/validations/recurrents\n  method: post\n  operationId: tokenizeCardForRecurring\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/purchases/recurrents\n  method: post\n  operationId: chargeRecurringToken\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paymentgateway/api/v1/refunds\n  method: post\n  operationId: createRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paymentgateway/api/v1/refunds/{refundReference}\n  method: get\n  operationId: getRefund\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction-search/api/v1/search/quick\n  method: get\n  operationId: quickTransactionSearch\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction-search/api/v1/search/reference\n  method: get\n  operationId: searchTransactionByReference\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction-search/api/v1/search/bulk\n  method: post\n  operationId: bulkTransactionSearch\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction-search/api/v1/transactions/{transactionId}\n  method: get\n  operationId: getTransactionDetail\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /quicktellerservice/api/v5/transactions/TransferFunds\n  method: post\n  operationId: sendSingleTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /quicktellerservice/api/v5/transactions/BulkTransfer\n\
  \  method: post\n  operationId: sendBulkTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /quicktellerservice/api/v5/transactions/NameInquiry\n  method: post\n  operationId: nameInquiry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /quicktellerservice/api/v5/banks\n  method: get\n  operationId: listBanks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /collections/w/pay\n  method: post\n  operationId: initiateWebRedirectPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collections/api/v1/gettransaction.json\n  method: get\n  operationId: getTransactionStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/interswitch/refs/heads/main/agentic-access/interswitch-agentic-access.yml
summary_line: 55 operations · 31 acting · 1 human-in-the-loop
tags:
- Payments
- Payment Infrastructure
- Card Network
- Verve
- Quickteller
- Webpay
- Bills Payment
- Transfers
- Lending
- Fintech
- Africa
- Nigeria
---
