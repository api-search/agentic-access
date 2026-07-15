---
acting_count: 25
action_class_counts:
  acting: 25
  connected: 38
api_specs:
- filename: tink-oauth-api-openapi.yml
  format: yaml
  label: Tink OAuth API
  slug: tink-oauth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tink-com/refs/heads/main/openapi/tink-oauth-api-openapi.yml
- filename: tink-account-check-api-openapi.yml
  format: yaml
  label: Tink Account Check API
  slug: tink-account-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tink-com/refs/heads/main/openapi/tink-account-check-api-openapi.yml
- filename: tink-data-api-openapi.yml
  format: yaml
  label: Tink Data API
  slug: tink-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tink-com/refs/heads/main/openapi/tink-data-api-openapi.yml
- filename: tink-data-enrichment-api-openapi.yml
  format: yaml
  label: Tink Data Enrichment API
  slug: tink-data-enrichment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tink-com/refs/heads/main/openapi/tink-data-enrichment-api-openapi.yml
- filename: tink-payments-api-openapi.yml
  format: yaml
  label: Tink Payments API
  slug: tink-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tink-com/refs/heads/main/openapi/tink-payments-api-openapi.yml
- filename: tink-risk-reports-api-openapi.yml
  format: yaml
  label: Tink Risk and Reports API
  slug: tink-risk-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tink-com/refs/heads/main/openapi/tink-risk-reports-api-openapi.yml
- filename: tink-money-manager-api-openapi.yml
  format: yaml
  label: Tink Money Manager API
  slug: tink-money-manager-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tink-com/refs/heads/main/openapi/tink-money-manager-api-openapi.yml
- filename: tink-connector-api-openapi.yml
  format: yaml
  label: Tink Connector API
  slug: tink-connector-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tink-com/refs/heads/main/openapi/tink-connector-api-openapi.yml
- filename: tink-webhooks-api-openapi.yml
  format: yaml
  label: Tink Webhooks API
  slug: tink-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/tink-com/refs/heads/main/openapi/tink-webhooks-api-openapi.yml
consequence_counts:
  physical: 4
  read: 38
  safety-critical: 1
  write: 20
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Tink Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /payments/mandates/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/mandates
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/{paymentId}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/{paymentId}/refunds
operation_count: 63
overview: 'Tink exposes 63 API operations that an AI agent could call, of which 25 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 38 read, 20 write, 4 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Tink
provider_slug: tink-com
slug: tink-com-agentic-access
source_filename: tink-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/tink-account-check-api-openapi.yml, openapi/tink-connector-api-openapi.yml,\n  openapi/tink-data-api-openapi.yml, openapi/tink-data-enrichment-api-openapi.yml, openapi/tink-money-manager-api-openapi.yml,\n  openapi/tink-oauth-api-openapi.yml, openapi/tink-payments-api-openapi.yml, openapi/tink-risk-reports-api-openapi.yml,\n  openapi/tink-webhooks-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 63\n  by_action_class:\n    connected: 38\n    acting: 25\n  by_consequence:\n    read: 38\n    write: 20\n    physical: 4\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /api/v1/account-verification-reports/{report_id}\n  method: get\n  operationId:\
  \ getAccountVerificationReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/account-verification-reports/{report_id}/pdf\n  method: get\n  operationId: getAccountVerificationReportPdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v1/business-account-verification-reports/{report_id}\n  method: get\n  operationId: getBusinessAccountVerificationReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /link/v1/session\n  method: post\n  operationId: createLinkSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connector/users/{external_user_id}/accounts\n  method: post\n  operationId: ingestConnectorAccounts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connector/users/{external_user_id}/transactions\n  method: post\n  operationId: ingestConnectorTransactions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /data/v2/accounts\n  method: get\n  operationId: listAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v2/accounts/{account_id}/balances\n  method: get\n  operationId: getAccountBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v2/accounts/{account_id}/parties\n  method: get\n  operationId: listAccountParties\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v2/transactions\n  method: get\n  operationId: listTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v2/identities\n  method: get\n  operationId: listIdentities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /data/v2/investment-accounts\n  method: get\n  operationId: listInvestmentAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v2/investment-accounts/{id}/holdings\n  method: get\n  operationId: listInvestmentHoldings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v2/loan-accounts\n  method: get\n  operationId: listLoanAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /data/v2/loan-accounts/{accountId}\n  method: get\n  operationId: getLoanAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/balance-refresh\n  method:\
  \ post\n  operationId: createBalanceRefresh\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/balance-refresh/{balanceRefreshId}\n  method: get\n  operationId: getBalanceRefresh\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/credentials/list\n  method: get\n  operationId: listCredentials\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/credentials/{credentialsId}\n  method: delete\n  operationId: deleteCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/provider-consents\n  method: get\n  operationId: listProviderConsents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /enrichment/v1/transactions\n  method: get\n  operationId: listEnrichedTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /enrichment/v1/categories\n  method: get\n  operationId: listCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /enrichment/v1/recurring-transactions\n  method: get\n  operationId: listRecurringTransactions\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /enrichment/v1/predicted-recurring-transactions\n  method: get\n  operationId: listPredictedRecurringTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /enrichment/v1/recurring-transactions-groups\n  method: get\n  operationId: listRecurringTransactionsGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /enrichment/v1/recurring-transactions-groups/{groupId}\n  method: get\n  operationId: getRecurringTransactionsGroup\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /finance-management/v1/cash-flow-summaries/{resolution}\n  method: get\n  operationId:\
  \ getCashFlowSummaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /finance-management/v1/business-budgets\n  method: post\n  operationId: createBusinessBudget\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /finance-management/v1/business-budgets\n  method: get\n  operationId: listBusinessBudgets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /finance-management/v1/business-budgets/{budgetId}\n  method: get\n  operationId: getBusinessBudget\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /finance-management/v1/business-budgets/{budgetId}\n  method: patch\n  operationId: updateBusinessBudget\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /finance-management/v1/business-budgets/{budgetId}\n  method: delete\n  operationId: deleteBusinessBudget\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /finance-management/v1/business-budgets/{budgetId}/history\n  method: get\n  operationId: getBusinessBudgetHistory\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /finance-management/v1/financial-calendar-events\n  method: post\n  operationId: createCalendarEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /finance-management/v1/financial-calendar-events\n  method: get\n  operationId: listCalendarEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /finance-management/v1/financial-calendar-events/{calendarEventId}\n  method: get\n  operationId: getCalendarEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /finance-management/v1/financial-calendar-events/{calendarEventId}\n  method: patch\n  operationId: updateCalendarEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /finance-management/v1/financial-calendar-events/{calendarEventId}\n  method: delete\n  operationId: deleteCalendarEvent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /finance-management/v1/financial-calendar-events/{calendarEventId}/reconciliations\n  method: post\n  operationId: createReconciliation\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /finance-management/v1/financial-calendar-summaries/{resolution}\n  method: get\n  operationId: listCalendarEventSummaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1/oauth/token\n  method: post\n  operationId: createOauthToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/oauth/authorization-grant\n  method: post\n  operationId: createAuthorizationGrant\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/oauth/authorization-grant/delegate\n  method: post\n  operationId: createDelegatedAuthorizationGrant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/user/create\n  method: post\n  operationId: createUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/user/delete\n\
  \  method: post\n  operationId: deleteUser\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments\n  method: post\n  operationId: initiatePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/{paymentId}\n  method: get\n  operationId: getPayment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/{paymentId}/cancel\n  method: post\n  operationId:\
  \ cancelPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/{paymentId}/refunds\n  method: post\n  operationId: refundPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/{paymentId}/refunds/{refundId}\n  method: get\n  operationId: getRefund\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /payments/mandates\n  method: post\n  operationId: createMandate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payments/mandates/{id}\n  method: get\n  operationId: getMandate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payments/mandates/{id}\n  method: delete\n  operationId: revokeMandate\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n\
  \    audit: required\n- path: /v2/income-checks/{report_id}\n  method: get\n  operationId: getIncomeCheckReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/income-checks/{report_id}:generate-pdf\n  method: get\n  operationId: generateIncomeCheckPdf\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /risk/v1/expense-checks/{report_id}\n  method: get\n  operationId: getExpenseCheckReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /risk/v1/risk-insights/{report_id}\n  method: get\n  operationId: getRiskInsightsReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n-\
  \ path: /risk/v2/risk-categorisation/reports/{report_id}\n  method: get\n  operationId: getRiskCategorisationReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/v2/webhook-endpoints\n  method: post\n  operationId: createWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/v2/webhook-endpoints\n  method: get\n  operationId: listWebhookEndpoints\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/v2/webhook-endpoints/{endpointId}\n  method: get\n  operationId: getWebhookEndpoint\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/v2/webhook-endpoints/{endpointId}\n  method: patch\n  operationId: updateWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /events/v2/webhook-endpoints/{endpointId}\n  method: delete\n  operationId: deleteWebhookEndpoint\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/tink-com/refs/heads/main/agentic-access/tink-com-agentic-access.yml
summary_line: 63 operations · 25 acting · 1 human-in-the-loop
tags:
- Open Banking
- PSD2
- Payment Initiation
- Account Aggregation
- Risk Decisioning
- Pay by Bank
- Finance
- Banking
- Europe
- Visa
---
