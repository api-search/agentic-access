---
acting_count: 70
action_class_counts:
  acting: 70
  connected: 148
api_specs:
- filename: lean-technologies-account-on-file-openapi.yml
  format: yaml
  label: Lean UAE Open Finance & Payments
  slug: lean-uae-open-finance-payments
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-technologies/refs/heads/main/openapi/lean-technologies-account-on-file-openapi.yml
- filename: lean-technologies-ksa-accounts-access-consents-openapi.yml
  format: yaml
  label: Lean KSA Open Banking
  slug: lean-ksa-open-banking
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/lean-technologies/refs/heads/main/openapi/lean-technologies-ksa-accounts-access-consents-openapi.yml
consequence_counts:
  physical: 29
  read: 148
  safety-critical: 1
  write: 40
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Lean Technologies Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /consents/v1/{consent_id}/revocation
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /customers/v1/{customer_id}/payment-sources/{payment_source_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /customers/v1/{customer_id}/payment-sources/{payment_source_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment-links/v1
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /payment-links/v1/{payment_link_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/account-on-file
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/v1/account-on-file
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/v1/destinations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/v1/destinations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/v1/intents
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/v1/intents
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payouts/refunds
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payouts/refunds
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /payouts/refunds
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payouts/v1/bulk-payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payouts/v1/bulk-payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payouts/v1/payment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payouts/v1/payment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payouts/v1/payment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payouts/v1/payment/destinations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payouts/v1/payment/destinations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payouts/v1/payment/destinations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payouts/v1/split-payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payouts/v1/split-payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /reconciliation/v1/payments
operation_count: 218
overview: 'Lean Technologies exposes 218 API operations that an AI agent could call, of which 70 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 148 read, 40 write, 29 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Lean Technologies
provider_slug: lean-technologies
slug: lean-technologies-agentic-access
source_filename: lean-technologies-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-19'\nmethod: generated\nsource: openapi/lean-technologies-account-on-file-openapi.yml, openapi/lean-technologies-bank-data-openapi.yml,\n  openapi/lean-technologies-banks-openapi.yml, openapi/lean-technologies-consents-openapi.yml,\n  openapi/lean-technologies-core-resources-openapi.yml, openapi/lean-technologies-customers-openapi.yml,\n  openapi/lean-technologies-data-openapi.yml, openapi/lean-technologies-enrichment-openapi.yml,\n  openapi/lean-technologies-entities-openapi.yml, openapi/lean-technologies-files-openapi.yml,\n  openapi/lean-technologies-insights-openapi.yml, openapi/lean-technologies-ksa-accounts-access-consents-openapi.yml,\n  openapi/lean-technologies-ksa-bank-data-openapi.yml, openapi/lean-technologies-ksa-core-resources-openapi.yml,\n  openapi/lean-technologies-ksa-customers-openapi.yml, openapi/lean-technologies-ksa-enrichment-openapi.yml,\n  openapi/lean-technologies-ksa-insights-openapi.yml, openapi/lean-technologies-ksa-open-banking-openapi.yml,\n\
  \  openapi/lean-technologies-ksa-payouts-openapi.yml, openapi/lean-technologies-ksa-reports-openapi.yml,\n  openapi/lean-technologies-ksa-verifications-openapi.yml, openapi/lean-technologies-payment-links-openapi.yml,\n  openapi/lean-technologies-payments-core-openapi.yml, openapi/lean-technologies-payments-customers-openapi.yml,\n  openapi/lean-technologies-payments-openapi.yml, openapi/lean-technologies-payouts-extended-openapi.yml,\n  openapi/lean-technologies-payouts-openapi.yml, openapi/lean-technologies-reconciliation-extended-openapi.yml,\n  openapi/lean-technologies-reconciliation-openapi.yml, openapi/lean-technologies-refunds-openapi.yml,\n  openapi/lean-technologies-schedules-openapi.yml, openapi/lean-technologies-sessions-openapi.yml,\n  openapi/lean-technologies-verifications-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n\
  \  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 218\n  by_action_class:\n    acting: 70\n    connected: 148\n  by_consequence:\n    write: 40\n    physical: 29\n    read: 148\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /consents/v1/account-on-file\n  method: post\n  operationId: createAccountOnFileConsent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/v1/account-on-file\n  method: post\n  operationId: initiateAccountOnFilePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/v1/{customer_id}/entities\n  method: get\n  operationId: getCustomerEntities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/v1/{customer_id}/entities/{entity_id}\n  method: get\n  operationId: getEntityById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/v1/{customer_id}/entities/{entity_id}\n  method: delete\n  operationId: deleteEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /data/v2/accounts\n  method: get\n  operationId: fetchAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v2/accounts/{account_id}/balances\n  method: get\n  operationId: fetchBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v2/accounts/{account_id}/transactions\n  method: get\n  operationId: fetchTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v2/identity\n  method: get\n  operationId: fetchCurrentIdentity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banks/v1\n  method: get\n  operationId: getBanks\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /consents/v1/{consent_id}\n  method: get\n  operationId: fetchConsent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /consents/v1/{consent_id}/balance\n  method: get\n  operationId: fetchConsentBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /consents/v1\n  method: get\n  operationId: fetchConsents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - api\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /consents/v1/{consent_id}/revocation\n  method: post\n  operationId: revokeConsent\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: safety-critical\n    subject: required\n    scope:\n    - api\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /customers/v1/\n  method: get\n  operationId: getCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/v1/\n  method: post\n  operationId: createCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/v1/{customer_id}/\n  method: get\n  operationId: getCustomerById\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/v1/{customer_id}/\n  method: put\n  operationId: updateCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/v1/app-user-id/{app_user_id}\n  method: get\n  operationId: getCustomerByUserId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banks/v1\n  method: get\n  operationId: getBanks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/v1\n  method: get\n  operationId: getEvents\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/v1/{customer_id}/entities\n  method: get\n  operationId: getCustomerEntities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/v1/{customer_id}/entities/{entity_id}\n  method: get\n  operationId: getEntityById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/v1/{customer_id}/entities/{entity_id}\n  method: delete\n  operationId: deleteEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /customers/v1/entities\n  method: get\n  operationId: listEntities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v2/accounts\n  method: get\n  operationId: fetchAccountsV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v2/accounts/{account_id}/balances\n  method: get\n  operationId: fetchBalancesV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v2/accounts/{account_id}/beneficiaries\n  method: get\n  operationId: fetchBeneficiariesV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v2/accounts/{account_id}/direct-debits\n  method:\
  \ get\n  operationId: fetchDirectDebits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v2/accounts/{account_id}/identities\n  method: get\n  operationId: fetchAllIdentities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v2/identity\n  method: get\n  operationId: fetchIdentitiesV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v2/refreshes\n  method: post\n  operationId: triggerDataRefresh\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /data/v2/refreshes\n  method: get\n  operationId: getDataRefreshes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v2/refreshes/{refresh_id}\n  method: get\n  operationId: getDataRefreshStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v2/results/{results_id}\n  method: get\n  operationId: getResultsV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v2/accounts/{account_id}/scheduled-payments\n  method: get\n  operationId: fetchScheduledPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v2/accounts/{account_id}/standing-orders\n\
  \  method: get\n  operationId: getStandingOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v2/accounts/{account_id}/transactions\n  method: get\n  operationId: fetchTransactionsV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/v2/income\n  method: post\n  operationId: getIncome\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /insights/v2/expenses\n  method: get\n  operationId: getExpenses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /customers/v1/{customer_id}/entities/{entity_id}\n  method: get\n  operationId: getEntityById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/v1/{customer_id}/entities/{entity_id}\n  method: delete\n  operationId: deleteEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/v1/{customer_id}/entities\n  method: get\n  operationId: getCustomerEntities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/v1/entities\n  method: get\n  operationId: listEntities\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /files/kyc/poa/{document_id}.pdf\n  method: get\n  operationId: getPoaDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/v3/account-controls\n  method: get\n  operationId: getAccountControls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/v2/assets/cashflows\n  method: get\n  operationId: getCashflows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/v2/assets/balances\n  method: get\n  operationId: getBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n   \
  \   max-ttl: 3600\n    audit: none\n- path: /insights/v3/behaviors\n  method: get\n  operationId: getBehavioralInsights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/v3/cashflow-patterns\n  method: get\n  operationId: getCashFlow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/v3/credit-assessments\n  method: get\n  operationId: getCreditAssessments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/v3/credit-obligations\n  method: get\n  operationId: getCreditObligationsV3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/v2/expenses\n\
  \  method: get\n  operationId: getExpenses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/v2/income\n  method: post\n  operationId: verifyIncome\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /insights/v2/liabilities/credit-obligations\n  method: get\n  operationId: getCreditObligations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/v2/liabilities/non-credit-obligations\n  method: get\n  operationId: getNonCreditObligations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/v2/customers/{customer_id}/reports/verification-of-income\n  method: post\n  operationId: createVerificationOfIncomeReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /insights/v2/customers/{customer_id}/reports/verification-of-income/{report_id}\n  method: get\n  operationId: getVerificationOfIncomeReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/v2/customers/{customer_id}/reports/bank-statements\n  method: post\n  operationId: createBankStatementsReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /insights/v2/customers/{customer_id}/reports/bank-statements/{report_id}\n  method: get\n  operationId: getBankStatementsReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/v1/name-verification\n  method: post\n  operationId: nameVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/accounts-access-consents\n  method: post\n  operationId: createConnectLink\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/v1/{customerId}/consents\n  method: get\n  operationId: getCustomerConsents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/v1/{customerId}/consents/{consentId}\n  method: get\n  operationId: getCustomerConsentById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v2/refreshes\n  method: post\n  operationId: trigger_data_refresh_v2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /customers/v1/entities\n  method: get\n  operationId: listEntities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/v1/{customer_id}/entities\n  method: get\n  operationId: getEntities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/v1/{customer_id}/entities/{entity_id}\n  method: get\n  operationId: getEntityById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/v1/{customer_id}/entities/{entity_id}\n  method: delete\n  operationId: deleteEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/v1/{customer_id}/entities/{entity_id}/consent/{consent_id}\n  method: delete\n  operationId: deleteConsent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/v2/accounts\n  method: get\n  operationId: fetchAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v2/accounts/{account_id}/balances\n  method: get\n  operationId: fetchBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /data/v2/accounts/{account_id}/transactions\n  method: get\n  operationId: fetchTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v2/identity\n  method: get\n  operationId: fetchCurrentIdentity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v2/accounts/{account_id}/identities\n  method: get\n  operationId: fetchAllIdentities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v2/accounts/{account_id}/beneficiaries\n  method: get\n  operationId: fetchBeneficiaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v2/accounts/{account_id}/direct-debits\n\
  \  method: get\n  operationId: fetchDirectDebits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v2/accounts/{account_id}/scheduled-payments\n  method: get\n  operationId: fetchScheduledPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v2/accounts/{account_id}/standing-orders\n  method: get\n  operationId: getStandingOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/v1\n  method: post\n  operationId: createCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /customers/v1\n  method: get\n  operationId: getCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/v1/{customer_id}\n  method: get\n  operationId: getCustomerById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/v1/app-user-id/{app_user_id}\n  method: get\n  operationId: getCustomerByAppUserId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banks/v1/\n  method: get\n  operationId: listBanks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v2/results/{results_id}\n  method:\
  \ get\n  operationId: getResults\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/v1/{customer_id}/entities\n  method: get\n  operationId: getCustomerEntities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/v1/{customer_id}/entities/{entity_id}\n  method: get\n  operationId: getEntityById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/v1/{customer_id}/entities/{entity_id}\n  method: delete\n  operationId: deleteEntity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n    \
  \  - abnormal\n      - high-value\n    audit: required\n- path: /customers/v1/entities\n  method: get\n  operationId: listEntities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/v2/income\n  method: post\n  operationId: getIncome\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /insights/v2/income/employment?async=true\n  method: get\n  operationId: getEmployment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/v2/assets/cashflows?async=true\n  method: get\n  operationId: GetCashflow\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/v2/assets/balances\n  method: get\n  operationId: getBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/v2/expenses\n  method: get\n  operationId: getExpenses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/v2/liabilities/credit-obligations\n  method: get\n  operationId: getCreditObligations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/v2/liabilities/non-credit-obligations\n  method: get\n  operationId: getNonCreditObligations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/v3/account-controls\n  method: get\n  operationId: getAccountControls\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/v2/assets/cashflows\n  method: get\n  operationId: getCashflows\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/v2/assets/balances\n  method: get\n  operationId: getBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/v3/behaviors\n  method: get\n  operationId: getBehavioralInsights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/v3/cashflow-patterns\n\
  \  method: get\n  operationId: getCashFlow\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/v3/credit-assessments\n  method: get\n  operationId: getCreditAssessments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/v3/credit-obligations\n  method: get\n  operationId: getCreditObligationsV3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/v2/expenses\n  method: get\n  operationId: getExpenses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/v2/assets/freelancers/cashflows\n  method: get\n  operationId: getFreelancersCashflows\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/v2/income\n  method: post\n  operationId: verifyIncome\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /insights/v2/income/employment\n  method: get\n  operationId: getEmploymentDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/v2/liabilities/credit-obligations\n  method: get\n  operationId: getCreditObligations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/v2/liabilities/non-credit-obligations\n\
  \  method: get\n  operationId: getNonCreditObligations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/v2/customers/{customer_id}/reports/verification-of-income\n  method: post\n  operationId: createVerificationOfIncomeReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /insights/v2/customers/{customer_id}/reports/verification-of-income/{report_id}\n  method: get\n  operationId: getVerificationOfIncomeReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /insights/v2/customers/{customer_id}/reports/bank-statements\n  method: post\n\
  \  operationId: createBankStatementsReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /insights/v2/customers/{customer_id}/reports/bank-statements/{report_id}\n  method: get\n  operationId: getBankStatementsReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /open-banking/account-information/2022.11.01-final-errata2/accounts/{AccountId}/parties\n  method: get\n  operationId: GetAccountPartiesV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /open-banking/account-information/2022.11.01-final-errata2/accounts\n  method: get\n  operationId:\
  \ GetAccountsV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /open-banking/account-information/2022.11.01-final-errata2/accounts/{AccountId}/balances\n  method: get\n  operationId: GetAccountBalancesV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /open-banking/account-information/2022.11.01-final-errata2/accounts/{AccountId}/beneficiaries\n  method: get\n  operationId: GetAccountBeneficiariesV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /open-banking/account-information/2022.11.01-final-errata2/accounts/{AccountId}/direct-debits\n  method: get\n  operationId: GetAccountDirectDebitsV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: o\n\n# --- truncated at 32 KB (62 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/lean-technologies/refs/heads/main/agentic-access/lean-technologies-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/lean-technologies/refs/heads/main/agentic-access/lean-technologies-agentic-access.yml
summary_line: 218 operations · 70 acting · 1 human-in-the-loop
tags:
- Open Banking
- Open Finance
- Payments
- Financial Data
- Fintech
- MENA
- UAE
- Saudi Arabia
- Pay by Bank
- Bank Data
- Account Verification
- Payouts
---
