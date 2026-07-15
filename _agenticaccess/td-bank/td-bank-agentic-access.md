---
acting_count: 7
action_class_counts:
  acting: 7
  connected: 25
api_specs:
- filename: td-bank-account-basic-api-openapi.yml
  format: yaml
  label: TD Bank Account Basic API
  slug: account-basic-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/openapi/td-bank-account-basic-api-openapi.yml
- filename: td-bank-account-detailed-api-openapi.yml
  format: yaml
  label: TD Bank Account Detailed API
  slug: account-detailed-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/openapi/td-bank-account-detailed-api-openapi.yml
- filename: td-bank-customer-api-openapi.yml
  format: yaml
  label: TD Bank Customer API
  slug: customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/openapi/td-bank-customer-api-openapi.yml
- filename: td-bank-transactions-api-openapi.yml
  format: yaml
  label: TD Bank Transactions API
  slug: transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/openapi/td-bank-transactions-api-openapi.yml
- filename: td-bank-statements-api-openapi.yml
  format: yaml
  label: TD Bank Statements API
  slug: statements-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/openapi/td-bank-statements-api-openapi.yml
- filename: td-bank-tax-forms-api-openapi.yml
  format: yaml
  label: TD Bank Tax Forms API
  slug: tax-forms-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/openapi/td-bank-tax-forms-api-openapi.yml
- filename: td-bank-bill-payment-api-openapi.yml
  format: yaml
  label: TD Bank Bill Payment API
  slug: bill-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/openapi/td-bank-bill-payment-api-openapi.yml
- filename: td-bank-rewards-api-openapi.yml
  format: yaml
  label: TD Bank Rewards API
  slug: rewards-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/openapi/td-bank-rewards-api-openapi.yml
- filename: td-bank-consent-api-openapi.yml
  format: yaml
  label: TD Bank Consent API
  slug: consent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/openapi/td-bank-consent-api-openapi.yml
- filename: td-bank-token-api-openapi.yml
  format: yaml
  label: TD Bank Token API
  slug: token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/openapi/td-bank-token-api-openapi.yml
- filename: td-bank-service-token-api-openapi.yml
  format: yaml
  label: TD Bank Service Token API
  slug: service-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/openapi/td-bank-service-token-api-openapi.yml
- filename: td-bank-apps-management-api-openapi.yml
  format: yaml
  label: TD Bank Apps Management API
  slug: apps-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/openapi/td-bank-apps-management-api-openapi.yml
- filename: td-bank-notifications-api-openapi.yml
  format: yaml
  label: TD Bank Notifications API
  slug: notifications-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/openapi/td-bank-notifications-api-openapi.yml
consequence_counts:
  read: 25
  safety-critical: 2
  write: 5
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Td Bank Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /consents/{consentId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /revoke
operation_count: 32
overview: 'TD Bank exposes 32 API operations that an AI agent could call, of which 7 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 25 read, 5 write, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: TD Bank
provider_slug: td-bank
slug: td-bank-agentic-access
source_filename: td-bank-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/td-bank-account-basic-api-openapi.yml, openapi/td-bank-account-detailed-api-openapi.yml,\n  openapi/td-bank-apps-management-api-openapi.yml, openapi/td-bank-bill-payment-api-openapi.yml,\n  openapi/td-bank-consent-api-openapi.yml, openapi/td-bank-customer-api-openapi.yml, openapi/td-bank-notifications-api-openapi.yml,\n  openapi/td-bank-rewards-api-openapi.yml, openapi/td-bank-service-token-api-openapi.yml, openapi/td-bank-statements-api-openapi.yml,\n  openapi/td-bank-tax-forms-api-openapi.yml, openapi/td-bank-token-api-openapi.yml, openapi/td-bank-transactions-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 32\n  by_action_class:\n    connected: 25\n    acting: 7\n\
  \  by_consequence:\n    read: 25\n    write: 5\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /accounts\n  method: get\n  operationId: listAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/contact\n  method: get\n  operationId: getAccountContact\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps\n  method: get\n  operationId: listApps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps\n  method:\
  \ post\n  operationId: createApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{appId}\n  method: get\n  operationId: getApp\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/{appId}\n  method: put\n  operationId: updateApp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /apps/{appId}/subscriptions\n  method: get\n  operationId: listAppSubscriptions\n  x-agentic-access:\n    action-class: connected\n \
  \   consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /apps/{appId}/clusters\n  method: get\n  operationId: listAppClusters\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clusters/{clusterId}/entities\n  method: get\n  operationId: listClusterEntities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/payees\n  method: get\n  operationId: listPayees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/bill-payments\n  method: get\n  operationId: listBillPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /consents/{consentId}\n  method: get\n  operationId: getConsent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /consents/{consentId}\n  method: delete\n  operationId: revokeConsent\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /consent-revocations\n  method: get\n  operationId: listConsentRevocations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/customers\n  method: get\n  operationId: listAccountCustomers\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/current\n  method: get\n  operationId: getCurrentCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notifications\n  method: get\n  operationId: listNotifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notifications/{notificationId}\n  method: get\n  operationId: getNotification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rewards-programs\n  method: get\n  operationId: listRewardsPrograms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /rewards-programs/{programId}\n  method: get\n  operationId: getRewardsProgram\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /service-token\n  method: post\n  operationId: createServiceToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/statements\n  method: get\n  operationId: listStatements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/statements/{statementId}\n  method: get\n  operationId: getStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/tax-forms\n  method: get\n  operationId: listTaxForms\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/tax-forms/{taxFormId}\n  method: get\n  operationId: getTaxForm\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /par\n  method: post\n  operationId: pushedAuthorizationRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /token\n  method: post\n  operationId: createToken\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /revoke\n  method: post\n  operationId: revokeToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /accounts/{accountId}/transactions\n  method: get\n  operationId: listTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/transactions/{transactionId}\n  method: get\n  operationId: getTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/transactions/{transactionId}/image\n  method: get\n  operationId: getTransactionImage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/td-bank/refs/heads/main/agentic-access/td-bank-agentic-access.yml
summary_line: 32 operations · 7 acting · 2 human-in-the-loop
tags:
- Account Aggregation
- AML
- Akoya
- Banking
- Bank Secrecy Act
- Bill Payment
- Consent
- Consumer Banking
- FDX
- Financial Services
- Merchant Solutions
- Notifications
- Open Banking
- Payments
- Rewards
- Tax Forms
- Token Management
- Transactions
---
