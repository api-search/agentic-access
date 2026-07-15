---
acting_count: 30
action_class_counts:
  acting: 30
api_specs:
- filename: okra-africa-openapi.yml
  format: yaml
  label: Okra Auth API
  slug: okra-africa-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-africa/refs/heads/main/openapi/okra-africa-openapi.yml
- filename: okra-africa-openapi.yml
  format: yaml
  label: Okra Accounts API
  slug: okra-africa-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-africa/refs/heads/main/openapi/okra-africa-openapi.yml
- filename: okra-africa-openapi.yml
  format: yaml
  label: Okra Balance API
  slug: okra-africa-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-africa/refs/heads/main/openapi/okra-africa-openapi.yml
- filename: okra-africa-openapi.yml
  format: yaml
  label: Okra Transactions API
  slug: okra-africa-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-africa/refs/heads/main/openapi/okra-africa-openapi.yml
- filename: okra-africa-openapi.yml
  format: yaml
  label: Okra Identity API
  slug: okra-africa-identity-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-africa/refs/heads/main/openapi/okra-africa-openapi.yml
- filename: okra-africa-openapi.yml
  format: yaml
  label: Okra Income API
  slug: okra-africa-income-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-africa/refs/heads/main/openapi/okra-africa-openapi.yml
- filename: okra-africa-openapi.yml
  format: yaml
  label: Okra Verification (KYC) API
  slug: okra-africa-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-africa/refs/heads/main/openapi/okra-africa-openapi.yml
- filename: okra-africa-openapi.yml
  format: yaml
  label: Okra Payments API
  slug: okra-africa-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-africa/refs/heads/main/openapi/okra-africa-openapi.yml
- filename: okra-africa-openapi.yml
  format: yaml
  label: Okra Banks API
  slug: okra-africa-banks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-africa/refs/heads/main/openapi/okra-africa-openapi.yml
- filename: okra-africa-openapi.yml
  format: yaml
  label: Okra Customers API
  slug: okra-africa-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-africa/refs/heads/main/openapi/okra-africa-openapi.yml
- filename: okra-africa-openapi.yml
  format: yaml
  label: Okra Wallet API
  slug: okra-africa-wallet-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-africa/refs/heads/main/openapi/okra-africa-openapi.yml
- filename: okra-africa-openapi.yml
  format: yaml
  label: Okra Reports API
  slug: okra-africa-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/okra-africa/refs/heads/main/openapi/okra-africa-openapi.yml
consequence_counts:
  physical: 5
  write: 25
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Okra Africa Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /authorization/initiate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /bulkfiles/initiate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pay/initiate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pay/link/create
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pay/verify
operation_count: 30
overview: 'Okra exposes 30 API operations that an AI agent could call, of which 30 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 25 write and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Okra
provider_slug: okra-africa
slug: okra-africa-agentic-access
source_filename: okra-africa-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/okra-africa-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 30\n  by_action_class:\n    acting: 30\n  by_consequence:\n    write: 25\n    physical: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /products/auths\n  method: post\n  operationId: retrieveAuth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /auth/getByCustomer\n  method: post\n  operationId: getAuthByCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products/accounts\n  method: post\n  operationId: retrieveAccounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/getByCustomer\n  method: post\n  operationId: getAccountsByCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /balance/check\n  method: post\n  operationId: checkBalance\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /balance/refresh\n  method: post\n  operationId: refreshBalance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transactions/process\n  method: post\n  operationId: processTransactions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transactions/refresh\n\
  \  method: post\n  operationId: refreshTransactions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products/transactions/download\n  method: post\n  operationId: downloadTransactions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products/identities\n  method: post\n  operationId: retrieveIdentity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n \
  \     - abnormal\n      - high-value\n    audit: required\n- path: /products/identity/merge\n  method: post\n  operationId: mergeIdentity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products/income/process\n  method: post\n  operationId: processIncome\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products/income/get\n  method: post\n  operationId: getIncome\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products/kyc/bvn-verify\n  method: post\n  operationId: verifyBvn\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products/kyc/nuban-verify\n  method: post\n  operationId: verifyNuban\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products/kyc/nuban-name-verify\n  method: post\n  operationId: verifyNubanName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products/kyc/tin-verify\n  method: post\n  operationId: verifyTin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /products/kyc/rc-verify\n  method: post\n  operationId: verifyRc\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pay/initiate\n  method: post\n  operationId: initiatePayment\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pay/verify\n  method: post\n  operationId: verifyPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pay/link/create\n  method: post\n  operationId: createPaymentLink\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /authorization/initiate\n  method: post\n  operationId: initiateAuthorization\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bulkfiles/initiate\n  method: post\n  operationId: initiateBulkPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /banks/list\n  method: post\n  operationId: listBanks\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /banks/getById\n  method: post\n  operationId: getBankById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/list\n  method: post\n  operationId: listCustomers\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/find-customers-by\n  method: post\n\
  \  operationId: findCustomersBy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/remove\n  method: post\n  operationId: removeCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /wallet/balance/check\n  method: post\n  operationId: checkWalletBalance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /reports/schedule\n  method: post\n  operationId: scheduleReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/okra-africa/refs/heads/main/agentic-access/okra-africa-agentic-access.yml
summary_line: 30 operations · 30 acting
tags:
- Open Banking
- Open Finance
- Financial Data
- Payments
- Fintech
- Account Linking
- Bank Data
- Africa
- Nigeria
- Financial Infrastructure
- Retired
---
