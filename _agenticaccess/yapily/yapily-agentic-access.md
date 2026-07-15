---
acting_count: 52
action_class_counts:
  acting: 52
  connected: 45
api_specs:
- filename: yapily-platform-api-openapi.yml
  format: yaml
  label: Yapily Platform API
  slug: yapily-platform-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yapily/refs/heads/main/openapi/yapily-platform-api-openapi.yml
- filename: yapily-institutions-api-openapi.yml
  format: yaml
  label: Yapily Institutions API
  slug: yapily-institutions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yapily/refs/heads/main/openapi/yapily-institutions-api-openapi.yml
- filename: yapily-consents-api-openapi.yml
  format: yaml
  label: Yapily Consents and Authorisations API
  slug: yapily-consents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yapily/refs/heads/main/openapi/yapily-consents-api-openapi.yml
- filename: yapily-data-api-openapi.yml
  format: yaml
  label: Yapily Data Access API (AIS)
  slug: yapily-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yapily/refs/heads/main/openapi/yapily-data-api-openapi.yml
- filename: yapily-payments-api-openapi.yml
  format: yaml
  label: Yapily Payments API (PIS)
  slug: yapily-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yapily/refs/heads/main/openapi/yapily-payments-api-openapi.yml
- filename: yapily-vrp-api-openapi.yml
  format: yaml
  label: Yapily Variable Recurring Payments API
  slug: yapily-vrp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yapily/refs/heads/main/openapi/yapily-vrp-api-openapi.yml
- filename: yapily-hosted-pages-api-openapi.yml
  format: yaml
  label: Yapily Hosted Pages API
  slug: yapily-hosted-pages-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yapily/refs/heads/main/openapi/yapily-hosted-pages-api-openapi.yml
- filename: yapily-data-plus-api-openapi.yml
  format: yaml
  label: Yapily Data Plus API
  slug: yapily-data-plus-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yapily/refs/heads/main/openapi/yapily-data-plus-api-openapi.yml
- filename: yapily-beneficiaries-api-openapi.yml
  format: yaml
  label: Yapily Beneficiaries API
  slug: yapily-beneficiaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/yapily/refs/heads/main/openapi/yapily-beneficiaries-api-openapi.yml
consequence_counts:
  physical: 18
  read: 45
  safety-critical: 2
  write: 32
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Yapily Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /hosted/vrp/consent-requests/{consentRequestId}/revoke
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /webhook/secrets/{webhook_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /bulk-payment-auth-requests
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /bulk-payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /embedded-bulk-payment-auth-requests
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /embedded-bulk-payment-auth-requests/{consentId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /embedded-payment-auth-requests
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /embedded-payment-auth-requests/{consentId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /hosted/payment-requests
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /hosted/payment-requests/links
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /hosted/vrp/consent-requests
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /hosted/vrp/consent-requests/{consentRequestId}/funds-confirmation
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /hosted/vrp/consent-requests/{consentRequestId}/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment-auth-requests
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /payment-auth-requests
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment-pre-auth-requests
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /variable-recurring-payments/funds-confirmation
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /variable-recurring-payments/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /variable-recurring-payments/sweeping/consents
operation_count: 97
overview: 'Yapily exposes 97 API operations that an AI agent could call, of which 52 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 45 read, 32 write, 18 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Yapily
provider_slug: yapily
slug: yapily-agentic-access
source_filename: yapily-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/yapily-beneficiaries-api-openapi.yml, openapi/yapily-consents-api-openapi.yml,\n  openapi/yapily-data-api-openapi.yml, openapi/yapily-data-plus-api-openapi.yml, openapi/yapily-hosted-pages-api-openapi.yml,\n  openapi/yapily-institutions-api-openapi.yml, openapi/yapily-payments-api-openapi.yml, openapi/yapily-platform-api-openapi.yml,\n  openapi/yapily-vrp-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 97\n  by_action_class:\n    acting: 52\n    connected: 45\n  by_consequence:\n    write: 32\n    read: 45\n    physical: 18\n    safety-critical: 2\n  human_in_the_loop_required: 2\noperations:\n- path: /applications/{applicationId}/beneficiaries\n  method: post\n  operationId:\
  \ createApplicationBeneficiary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{applicationId}/beneficiaries\n  method: get\n  operationId: getApplicationBeneficiaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationId}/beneficiaries/{beneficiaryId}\n  method: get\n  operationId: getApplicationBeneficiaryById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationId}/beneficiaries/{beneficiaryId}\n  method: delete\n  operationId: deleteApplicationBeneficiaryById\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{userId}/beneficiaries\n  method: post\n  operationId: createUserBeneficiary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{userId}/beneficiaries\n  method: get\n  operationId: getUserBeneficiaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{userId}/beneficiaries/{beneficiaryId}\n  method: patch\n  operationId: patchUserBeneficiary\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{userId}/beneficiaries/{beneficiaryId}\n  method: get\n  operationId: getUserBeneficiary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users/{userId}/beneficiaries/{beneficiaryId}\n  method: delete\n  operationId: deleteUserBeneficiary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{userId}/beneficiaries/{beneficiaryId}/approve\n  method: post\n  operationId: approveBeneficiary\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{userId}/beneficiaries/{beneficiaryId}/reject\n  method: post\n  operationId: rejectBeneficiary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account-auth-requests\n  method: patch\n  operationId: reAuthoriseAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /account-auth-requests\n  method: post\n  operationId: initiateAccountRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /account-auth-requests\n  method: put\n  operationId: updatePreAuthoriseAccountConsent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bulk-payment-auth-requests\n  method: post\n  operationId: createBulkPaymentAuthorisation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange:\
  \ true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /consent-auth-code\n  method: post\n  operationId: createConsentWithCode\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /consent-one-time-token\n  method: post\n  operationId: getConsentBySingleAccessConsent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /consents\n  method: get\n  operationId: getConsents\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /consents/{consentId}\n  method: delete\n  operationId: delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /consents/{consentId}\n  method: get\n  operationId: getConsentById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /consents/{consentId}/extend\n  method: post\n  operationId: extendConsent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /embedded-account-auth-requests\n  method: post\n  operationId: initiateEmbeddedAccountRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /embedded-account-auth-requests/{consentId}\n  method: put\n  operationId: updateEmbeddedAccountRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /embedded-bulk-payment-auth-requests\n  method: post\n  operationId: createEmbeddedBulkPaymentAuthorisation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /embedded-bulk-payment-auth-requests/{consentId}\n  method: put\n  operationId: updateEmbeddedBulkPaymentAuthorisation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /embedded-payment-auth-requests\n  method: post\n  operationId: createEmbeddedPaymentAuthorisation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n \
  \     purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /embedded-payment-auth-requests/{consentId}\n  method: put\n  operationId: updateEmbeddedPaymentAuthorisation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment-auth-requests\n  method: post\n  operationId: createPaymentAuthorisation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n     \
  \ - high-value\n    audit: required\n- path: /payment-auth-requests\n  method: put\n  operationId: updatePaymentAuthorisation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pre-auth-requests\n  method: post\n  operationId: createPreAuthorisationRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment-pre-auth-requests\n  method: post\n  operationId: createPaymentPreAuthorisationRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts\n  method: get\n  operationId: getAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/balances\n  method: get\n  operationId: getAccountBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/beneficiaries\n  method: get\n  operationId: getBeneficiaries\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/direct-debits\n  method: get\n  operationId: getAccountDirectDebits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/periodic-payments\n  method: get\n  operationId: getAccountPeriodicPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/scheduled-payments\n  method: get\n  operationId: getAccountScheduledPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/statements\n  method: get\n  operationId: getStatements\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/statements/{statementId}\n  method: get\n  operationId: getStatement\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/statements/{statementId}/file\n  method: get\n  operationId: getStatementFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/transactions\n  method: get\n  operationId: getTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /identity\n  method: get\n  operationId: getIdentity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/real-time/transactions\n  method: get\n  operationId: getRealTimeTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountId}/transactions/categorisation\n  method: post\n  operationId: post-accounts-accountId-transactions-categorisation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{accountId}/transactions/categorisation/{categorisationId}\n  method: get\n  operationId: get-accounts-transactions-categorised\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /transactions/categorisation\n  method: post\n  operationId: post-transactions-categorisation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transactions/categorisation/{categorisationId}\n  method: get\n  operationId: get-transactions-categorised\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/categorisation/categories/{accountType}\n  method: get\n  operationId: get-categorisation-accountType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hosted/consent-requests\n  method: post\n\
  \  operationId: createHostedConsentRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hosted/consent-requests/{consentRequestId}\n  method: get\n  operationId: getHostedConsentRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hosted/payment-requests\n  method: post\n  operationId: createHostedPaymentRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /hosted/payment-requests/links\n  method: post\n  operationId: createHostedPaymentRequestLink\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hosted/payment-requests/{paymentRequestId}\n  method: get\n  operationId: getHostedPaymentRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hosted/vrp/consent-requests\n  method: post\n  operationId: createHostedVRPConsentRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hosted/vrp/consent-requests\n  method: get\n  operationId: getHostedVRPConsentRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hosted/vrp/consent-requests/{consentRequestId}\n  method: get\n  operationId: getHostedVrpConsentRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hosted/vrp/consent-requests/{consentRequestId}/revoke\n  method: post\n  operationId: revokeHostedConsentRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /hosted/vrp/consent-requests/{consentRequestId}/payments\n  method: post\n  operationId: createHostedVrpPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /hosted/vrp/consent-requests/{consentRequestId}/payments/{paymentId}\n  method: get\n  operationId: getHostedVRPPaymentRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /hosted/vrp/consent-requests/{consentRequestId}/funds-confirmation\n  method: post\n  operationId: createHostedVrpFundsConfirmation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /institutions\n  method: get\n  operationId: getInstitutions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /institutions/{institutionId}\n  method: get\n  operationId: getInstitution\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bulk-payments\n  method: post\n  operationId: createBulkPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /bulk-payments/{bulkPaymentId}\n  method: get\n  operationId: getBulkPaymentStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /bulk-payments/{bulkPaymentId}/details\n  method: get\n  operationId: getBulkPaymentDetailsById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments\n  method: post\n  operationId: createPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /payments/{paymentId}/details\n  method: get\n  operationId: getPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users\n  method: get\n  operationId: getUsers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /users\n  method: post\n  operationId: addUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{userUuid}\n  method: patch\n  operationId: patchUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n   \
  \   human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{userUuid}\n  method: delete\n  operationId: deleteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /users/{userUuid}\n  method: get\n  operationId: getUser\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notifications/event-subscriptions\n  method: post\n  operationId: createEventSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /notifications/event-subscriptions\n  method: get\n  operationId: getEventSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notifications/event-subscriptions/{eventTypeId}\n  method: get\n  operationId: getEventSubscriptionById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /notifications/event-subscriptions/{eventTypeId}\n  method: delete\n  operationId: deleteEventSubscriptionById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /institutions/constraints/payments\n  method: get\n\
  \  operationId: getPaymentConstraintsRulesByInstitution\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /institutions/constraints/data\n  method: get\n  operationId: getAccountConstraintsRulesByInstitution\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications\n  method: post\n  operationId: createSubApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications\n  method: get\n  operationId: searchApplications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n     \
  \ max-ttl: 3600\n    audit: none\n- path: /applications/{applicationId}\n  method: get\n  operationId: getApplicationById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /applications/{applicationId}\n  method: put\n  operationId: updateApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{applicationId}\n  method: delete\n  operationId: deleteApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /applications/{applicationId}/vrp\n  method: post\n  operationId: createApplicationVRPConfigurationByApplicationId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{applicationId}/vrp\n  method: put\n  operationId: updateApplicationVRPConfigurationByApplicationId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /applications/{applicationId}/vrp\n  method: get\n  operationId: getApplicationVRPConfigurationByApplicationId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook/events/categories\n  method: get\n  operationId: getWebhookEventsCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook/events\n  method: post\n  operationId: registerWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook/events\n  method: get\n  operationId: getRegisteredWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhook/events/{webhook_id}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /webhook/secrets/{webhook_id}\n  method: post\n  operationId: webhookSecretReset\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /variable-recurring-payments/sweeping/consents\n  method: post\n  operationId: createSweepingAuthorisation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /variable-recurring-payments/sweeping/consents/{consentId}\n  method: get\n  operationId: getSweepingVrpConsentById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /variable-recurring-payments/funds-confirmation\n  method: post\n  operationId: createVrpFundsConfirmation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /variable-recurring-payments/payments\n  method: post\n  operationId: createVrpPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /variable-recurring-payments/payments/{paymentId}/details\n  method: get\n  operationId: getVrpPaymentDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/yapily/refs/heads/main/agentic-access/yapily-agentic-access.yml
summary_line: 97 operations · 52 acting · 2 human-in-the-loop
tags:
- Open Banking
- AISP
- PISP
- Payments
- Account Information
- Variable Recurring Payments
- Financial Services
- PSD2
- FCA
- Berlin Group
- UK
- Europe
- FinTech
---
