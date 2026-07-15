---
acting_count: 33
action_class_counts:
  acting: 33
  connected: 30
api_specs:
- filename: monnify-authentication-api-openapi.yml
  format: yaml
  label: Monnify Authentication API
  slug: monnify-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/monnify-authentication-api-openapi.yml
- filename: monnify-collections-api-openapi.yml
  format: yaml
  label: Monnify Collections API
  slug: monnify-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/monnify-collections-api-openapi.yml
- filename: monnify-reserved-accounts-api-openapi.yml
  format: yaml
  label: Monnify Reserved Accounts API
  slug: monnify-reserved-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/monnify-reserved-accounts-api-openapi.yml
- filename: monnify-disbursements-api-openapi.yml
  format: yaml
  label: Monnify Disbursements API
  slug: monnify-disbursements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/monnify-disbursements-api-openapi.yml
- filename: monnify-sub-accounts-api-openapi.yml
  format: yaml
  label: Monnify Sub-Accounts API
  slug: monnify-sub-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/monnify-sub-accounts-api-openapi.yml
- filename: monnify-direct-debit-api-openapi.yml
  format: yaml
  label: Monnify Direct Debit API
  slug: monnify-direct-debit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/monnify-direct-debit-api-openapi.yml
- filename: monnify-invoices-api-openapi.yml
  format: yaml
  label: Monnify Invoices API
  slug: monnify-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/monnify-invoices-api-openapi.yml
- filename: monnify-bills-payment-api-openapi.yml
  format: yaml
  label: Monnify Bills Payment API
  slug: monnify-bills-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/monnify-bills-payment-api-openapi.yml
- filename: monnify-verification-api-openapi.yml
  format: yaml
  label: Monnify Verification API
  slug: monnify-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/monnify-verification-api-openapi.yml
- filename: monnify-wallets-api-openapi.yml
  format: yaml
  label: Monnify Wallets API
  slug: monnify-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/monnify-wallets-api-openapi.yml
- filename: monnify-refunds-api-openapi.yml
  format: yaml
  label: Monnify Refunds API
  slug: monnify-refunds-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/monnify-refunds-api-openapi.yml
- filename: monnify-settlements-api-openapi.yml
  format: yaml
  label: Monnify Settlements API
  slug: monnify-settlements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/monnify-settlements-api-openapi.yml
- filename: moniepoint-pos-api-openapi.yml
  format: yaml
  label: Moniepoint POS Push Payment API
  slug: moniepoint-pos-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/openapi/moniepoint-pos-api-openapi.yml
consequence_counts:
  physical: 18
  read: 30
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Moniepoint Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/bank-transfer/reserved-accounts/limit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/v1/bank-transfer/reserved-accounts/limit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/bill-payment/customer-validate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/bill-payment/process-bill
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/invoice/create
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/v1/invoice/{invoiceReference}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/merchant/bank-transfer/init-payment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/merchant/cards/charge
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/merchant/cards/charge-card-token
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/push-payment/request
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1/refunds/initiate-refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/bank-transfer/reserved-accounts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /api/v2/bank-transfer/reserved-accounts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /api/v2/bank-transfer/reserved-accounts/{accountReference}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/disbursements/bulk
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/disbursements/single
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/disbursements/single/resend-otp
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v2/disbursements/single/validate-otp
operation_count: 63
overview: 'Moniepoint exposes 63 API operations that an AI agent could call, of which 33 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 30 read, 15 write, and 18 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Moniepoint
provider_slug: moniepoint
slug: moniepoint-agentic-access
source_filename: moniepoint-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/moniepoint-pos-api-openapi.yml, openapi/monnify-authentication-api-openapi.yml,\n  openapi/monnify-bills-payment-api-openapi.yml, openapi/monnify-collections-api-openapi.yml,\n  openapi/monnify-direct-debit-api-openapi.yml, openapi/monnify-disbursements-api-openapi.yml,\n  openapi/monnify-invoices-api-openapi.yml, openapi/monnify-refunds-api-openapi.yml, openapi/monnify-reserved-accounts-api-openapi.yml,\n  openapi/monnify-settlements-api-openapi.yml, openapi/monnify-sub-accounts-api-openapi.yml,\n  openapi/monnify-verification-api-openapi.yml, openapi/monnify-wallets-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 63\n  by_action_class:\n    acting: 33\n    connected:\
  \ 30\n  by_consequence:\n    physical: 18\n    read: 30\n    write: 15\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/push-payment/request\n  method: post\n  operationId: pushPaymentRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/push-payment/status/{reference}\n  method: get\n  operationId: pushPaymentStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/auth/login\n  method: post\n  operationId: monnifyLogin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/bill-payment/categories\n  method: get\n  operationId: listBillCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/bill-payment/billers\n  method: get\n  operationId: listBillers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/bill-payment/biller-items\n  method: get\n  operationId: listBillerItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/bill-payment/customer-validate\n  method: post\n  operationId: validateBillsCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/bill-payment/process-bill\n  method: post\n  operationId: processBill\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/bill-payment/status\n  method: get\n  operationId: getBillStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/merchant/transactions/init-transaction\n  method: post\n  operationId: initializeTransaction\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/merchant/bank-transfer/init-payment\n  method: post\n  operationId: payWithBankTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/merchant/cards/charge\n  method: post\n  operationId: chargeCard\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n \
  \   escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/merchant/cards/otp/authorize\n  method: post\n  operationId: authorizeOtp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/merchant/cards/charge-card-token\n  method: post\n  operationId: chargeCardToken\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/merchant/transactions/query\n  method: get\n  operationId:\
  \ getTransactionStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/transactions/search\n  method: get\n  operationId: searchTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/direct-debit/mandate\n  method: post\n  operationId: createMandate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/direct-debit/mandate/{mandateCode}\n  method: get\n  operationId: getMandate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /api/v1/direct-debit/mandate/{mandateCode}\n  method: delete\n  operationId: cancelMandate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/direct-debit/mandate/activation\n  method: post\n  operationId: activateMandate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/direct-debit/mandate/debit\n  method: post\n  operationId: debitMandate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/disbursements/single\n  method: post\n  operationId: initiateSingleTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/disbursements/single/validate-otp\n  method: post\n  operationId: authorizeSingleTransferOtp\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/disbursements/single/resend-otp\n\
  \  method: post\n  operationId: resendTransferOtp\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/disbursements/single/summary\n  method: get\n  operationId: getSingleTransferStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/disbursements/single/transactions\n  method: get\n  operationId: listSingleTransfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/disbursements/bulk\n  method: post\n  operationId: initiateBulkTransfer\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/disbursements/bulk/summary\n  method: get\n  operationId: getBulkTransferSummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/disbursements/bulk/{batchReference}/transactions\n  method: get\n  operationId: listBulkTransferItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/disbursements/wallet-balance\n  method: get\n  operationId: getWalletBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /api/v1/sdk/transactions/banks\n  method: get\n  operationId: listBanks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/disbursements/account/validate\n  method: get\n  operationId: validateBankAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/invoice/create\n  method: post\n  operationId: createInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/invoice/{invoiceReference}/details\n  method: get\n  operationId:\
  \ getInvoice\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/invoice/all\n  method: get\n  operationId: listInvoices\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/invoice/{invoiceReference}/cancel\n  method: delete\n  operationId: cancelInvoice\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/refunds/initiate-refund\n  method: post\n  operationId: initiateRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/refunds\n  method: get\n  operationId: listRefunds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/refunds/{refundReference}\n  method: get\n  operationId: getRefundStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/bank-transfer/reserved-accounts\n  method: post\n  operationId: reserveAccountV2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/bank-transfer/reserved-accounts\n  method: put\n  operationId: updateReservedAccountKyc\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/bank-transfer/reserved-accounts/{accountReference}\n  method: get\n  operationId: getReservedAccountV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2/bank-transfer/reserved-accounts/{accountReference}\n  method: delete\n  operationId: deallocateReservedAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n   \
  \ subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/bank-transfer/reserved-accounts/transactions\n  method: get\n  operationId: listReservedAccountTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/bank-transfer/reserved-accounts/limit\n  method: post\n  operationId: reserveAccountWithLimit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/bank-transfer/reserved-accounts/limit\n\
  \  method: put\n  operationId: updateReservedAccountLimit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/limit-profiles\n  method: post\n  operationId: createLimitProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/limit-profiles\n  method: get\n  operationId: listLimitProfiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/limit-profiles\n\
  \  method: put\n  operationId: updateLimitProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/transactions/find-by-settlement-reference\n  method: get\n  operationId: findTransactionsBySettlement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/settlements\n  method: get\n  operationId: listSettlements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sub-accounts\n  method: post\n  operationId: createSubAccounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sub-accounts\n  method: put\n  operationId: updateSubAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/sub-accounts\n  method: get\n  operationId: listSubAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/sub-accounts/{subAccountCode}\n  method: delete\n  operationId: deleteSubAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/disbursements/account/validate\n  method: get\n  operationId: validateAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/vas/bvn-account-match\n  method: post\n  operationId: matchBvnToAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/vas/bvn-details/{bvn}\n  method: get\n  operationId: getBvnDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/vas/verify-nin\n  method: post\n\
  \  operationId: verifyNin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/disbursements/wallet\n  method: post\n  operationId: createWallet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/disbursements/wallet\n  method: get\n  operationId: listWallets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/disbursements/wallet-balance\n  method: get\n  operationId: getWalletBalance\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/disbursements/wallet/transactions\n  method: get\n  operationId: listWalletTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/moniepoint/refs/heads/main/agentic-access/moniepoint-agentic-access.yml
summary_line: 63 operations · 33 acting
tags:
- Africa
- Nigeria
- Payments
- Banking
- Fintech
- Acquiring
- POS
- Collections
- Disbursements
- Virtual Accounts
- Direct Debit
- Bills Payment
- SMB
- Working Capital
- Unicorn
---
