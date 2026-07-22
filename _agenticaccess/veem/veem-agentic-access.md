---
acting_count: 27
action_class_counts:
  acting: 27
  connected: 23
api_specs:
- filename: veem-api-openapi.yml
  format: yaml
  label: Veem Public API
  slug: veem-public-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/veem/refs/heads/main/openapi/veem-api-openapi.yml
consequence_counts:
  read: 23
  safety-critical: 27
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 27
kind: agentic-access
layout: agentic-access
method: generated
name: Veem Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /veem/v1.0/payments/cryptowallet/payin
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /veem/v1.0/payments/cryptowallet/payout
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /veem/v1.0/payments/wallet/addFunds
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /veem/v1.0/payments/wallet/withdraw
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /veem/v1.2/account
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /veem/v1.2/account/bank-account
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /veem/v1.2/account/bank-account/{bankAccountId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /veem/v1.2/account/{accountId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /veem/v1.2/account/{accountId}/setting
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /veem/v1.2/attachments
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /veem/v1.2/beneficial-ownership
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /veem/v1.2/claimless-payments
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /veem/v1.2/contacts
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /veem/v1.2/contacts/batch
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /veem/v1.2/crypto-wallet/applications
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /veem/v1.2/crypto-wallet/applications/{applicationId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /veem/v1.2/crypto-wallet/applications/{applicationId}/add-currency
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /veem/v1.2/exchangerates/quote/enhanced
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /veem/v1.2/exchangerates/quote/enhanced-1
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /veem/v1.2/invoices
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /veem/v1.2/invoices/{invoiceId}/approve
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /veem/v1.2/invoices/{invoiceId}/cancel
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /veem/v1.2/payments
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /veem/v1.2/payments/{paymentId}/approve
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /veem/v1.2/webhooks
operation_count: 50
overview: 'Veem exposes 50 API operations that an AI agent could call, of which 27 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 23 read and 27 safety-critical.


  27 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Veem
provider_slug: veem
slug: veem-agentic-access
source_filename: veem-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/veem-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 50\n  by_action_class:\n    acting: 27\n    connected: 23\n  by_consequence:\n    safety-critical: 27\n    read: 23\n  human_in_the_loop_required: 27\noperations:\n- path: /veem/v1.2/account/bank-account\n  method: post\n  operationId: addBankAccountUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /veem/v1.2/crypto-wallet/applications/{applicationId}/add-currency\n\
  \  method: post\n  operationId: addCryptoWalletApplicationCurrency\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /veem/v1.2/invoices/{invoiceId}/approve\n  method: post\n  operationId: approveInvoiceUsingPOST_2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /veem/v1.2/payments/{paymentId}/approve\n  method: post\n  operationId: approvePaymentUsingPOST_2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /veem/v1.2/invoices/{invoiceId}/cancel\n  method: post\n  operationId: cancelInvoiceUsingPOST_2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /veem/v1.2/account\n  method: post\n  operationId: createAccountUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /veem/v1.2/beneficial-ownership\n  method: post\n  operationId: createBoiUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /veem/v1.2/beneficial-ownership\n  method: get\n  operationId: getBoiUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /veem/v1.2/claimless-payments\n  method: post\n  operationId: createClaimLessPaymentUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /veem/v1.2/contacts/batch\n  method: post\n  operationId: createContactsUsingPOST_2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /veem/v1.2/contacts\n  method: post\n  operationId: createContactUsingPOST_2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /veem/v1.2/contacts\n  method: get\n  operationId: getContactsUsingGET_2\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /veem/v1.2/crypto-wallet/applications\n  method: post\n  operationId: createCryptoWalletApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /veem/v1.0/payments/cryptowallet/payin\n  method: post\n  operationId: createCryptoWalletPayin\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /veem/v1.0/payments/cryptowallet/payout\n\
  \  method: post\n  operationId: createCryptoWalletPayout\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /veem/v1.2/invoices\n  method: post\n  operationId: createInvoiceUsingPOST_2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /veem/v1.2/account/{accountId}/setting\n  method: post\n  operationId: createOrUpdateAccountSettingsUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /veem/v1.2/payments\n  method: post\n  operationId: createPaymentUsingPOST_2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /veem/v1.2/webhooks\n  method: post\n  operationId: createWebhookUsingPOST_2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n-\
  \ path: /veem/v1.2/webhooks\n  method: get\n  operationId: getWebhooksUsingGET_2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /veem/v1.2/webhooks/{webhookId}\n  method: delete\n  operationId: deleteWebhookUsingDELETE_2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /veem/v1.2/webhooks/{webhookId}\n  method: get\n  operationId: getWebhookUsingGET_2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /veem/v1.2/webhooks/{webhookId}\n  method: patch\n  operationId: updateWebhookUsingPATCH_2\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /veem/v1.2/attachments\n  method: get\n  operationId: downloadAttachmentUsingGET_2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /veem/v1.2/attachments\n  method: post\n  operationId: uploadAttachmentUsingPOST_2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /veem/v1.2/account/{accountId}\n  method: patch\n  operationId:\
  \ editAccountUsingPATCH\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /veem/v1.2/account/{accountId}\n  method: get\n  operationId: getAccountUsingGET\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /veem/v1.2/account/bank-account/{bankAccountId}\n  method: patch\n  operationId: editBankAccountUsingPATCH\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n\
  - path: /veem/v1.2/contacts/batch/{batchId}\n  method: get\n  operationId: getContactBatchUsingGET_2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /veem/v1.2/contacts/{contactId}\n  method: get\n  operationId: getContactUsingGET_2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /veem/public/v1.2/country-currency-map\n  method: get\n  operationId: getCountryCurrencyMapUsingGET_2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /veem/v1.2/crypto-wallet/applications/{applicationId}\n  method: get\n  operationId: getCryptoWalletApplication\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /veem/v1.2/crypto-wallet/applications/{applicationId}\n  method: patch\n  operationId: patchCryptoWalletApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /veem/v1.2/crypto-wallet/applications/{applicationId}/routes/{routeId}\n  method: get\n  operationId: getCryptoWalletApplicationRoute\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /veem/v1.2/crypto-wallet/applications/{applicationId}/routes\n  method: get\n  operationId: getCryptoWalletApplicationRoutes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /veem/v1.2/crypto-wallet/balance/{fundingMethodId}\n  method: get\n  operationId: getCryptoWalletBalanceById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /veem/v1.2/crypto-wallet/balance\n  method: get\n  operationId: getCryptoWalletBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /veem/v1.2/crypto-wallet/details\n  method: get\n  operationId: getCryptoWalletDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /veem/v1.2/crypto-wallet/details/{fundingMethodId}\n  method: get\n  operationId: getCryptoWalletDetailsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /veem/v1.2/crypto-wallet\n  method: get\n  operationId: getCryptoWallets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /veem/v1.2/crypto-wallet/transactions/{fundingMethodId}\n  method: get\n  operationId: getCryptoWalletTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /veem/v1.2/wallets\n  method: get\n  operationId: getFundingMethodsUsingGET_3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /veem/v1.2/wallets/{walletId}\n  method: get\n  operationId: getFundingMethodsUsingGET_6\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /veem/v1.2/invoices/{invoiceId}\n  method: get\n  operationId: getInvoiceUsingGET_2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /veem/v1.2/payments/{paymentId}\n  method: get\n  operationId: getPaymentUsingGET_2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /veem/v1.2/exchangerates/quote/enhanced-1\n  method: post\n  operationId: getQuoteEnhancedUsingPOST-1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /veem/v1.2/exchangerates/quote/enhanced\n  method: post\n  operationId: getQuoteEnhancedUsingPOST\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /veem/v1.2/customers\n  method: get\n  operationId: searchCustomersUsingGET_2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /veem/v1.0/payments/wallet/addFunds\n  method: post\n  operationId: walletAddFundsUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /veem/v1.0/payments/wallet/withdraw\n\
  \  method: post\n  operationId: walletWithdrawUsingPOST\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/veem/refs/heads/main/agentic-access/veem-agentic-access.yml
summary_line: 50 operations · 27 acting · 27 human-in-the-loop
tags:
- Payments
- B2B Payments
- Cross-Border Payments
- Invoicing
- Wallets
- Fintech
- Global Payments
---
