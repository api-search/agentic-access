---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 26
api_specs:
- filename: inscribe-bank-accounts-api-openapi.yml
  format: yaml
  label: Inscribe Bank Accounts API
  slug: inscribe-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inscribe/refs/heads/main/openapi/inscribe-bank-accounts-api-openapi.yml
- filename: inscribe-collect-sessions-api-openapi.yml
  format: yaml
  label: Inscribe Collect Sessions API
  slug: inscribe-collect-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inscribe/refs/heads/main/openapi/inscribe-collect-sessions-api-openapi.yml
- filename: inscribe-credit-insights-api-openapi.yml
  format: yaml
  label: Inscribe Credit Insights API
  slug: inscribe-credit-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inscribe/refs/heads/main/openapi/inscribe-credit-insights-api-openapi.yml
- filename: inscribe-customers-api-openapi.yml
  format: yaml
  label: Inscribe Customers API
  slug: inscribe-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inscribe/refs/heads/main/openapi/inscribe-customers-api-openapi.yml
- filename: inscribe-documents-api-openapi.yml
  format: yaml
  label: Inscribe Documents API
  slug: inscribe-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inscribe/refs/heads/main/openapi/inscribe-documents-api-openapi.yml
- filename: inscribe-open-banking-api-openapi.yml
  format: yaml
  label: Inscribe Open Banking API
  slug: inscribe-open-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inscribe/refs/heads/main/openapi/inscribe-open-banking-api-openapi.yml
- filename: inscribe-reachability-check-api-openapi.yml
  format: yaml
  label: Inscribe Reachability Check API
  slug: inscribe-reachability-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inscribe/refs/heads/main/openapi/inscribe-reachability-check-api-openapi.yml
- filename: inscribe-transactions-api-openapi.yml
  format: yaml
  label: Inscribe Transactions API
  slug: inscribe-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/inscribe/refs/heads/main/openapi/inscribe-transactions-api-openapi.yml
consequence_counts:
  read: 26
  write: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Inscribe Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 43
overview: 'Inscribe exposes 43 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 26 read and 17 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Inscribe
provider_slug: inscribe
slug: inscribe-agentic-access
source_filename: inscribe-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/inscribe-core-resources-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 43\n  by_action_class:\n    acting: 17\n    connected: 26\n  by_consequence:\n    write: 17\n    read: 26\n  human_in_the_loop_required: 0\noperations:\n- path: /collect/sessions\n  method: post\n  operationId: createSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collect/sessions\n  method: get\n  operationId: getCollectSessions\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collect/sessions/{session_id}\n  method: get\n  operationId: getCollectSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /collect/sessions/{session_id}\n  method: put\n  operationId: updateCollectSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collect/sessions/{session_id}/document_requests\n  method: post\n  operationId: addDocumentRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /collect/sessions/{session_id}/document_requests/{document_request_id}\n  method: delete\n  operationId: deleteDocumentRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers\n  method: post\n  operationId: addCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers\n  method: get\n  operationId: getCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customer_id}\n  method: get\n  operationId: getCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customer_id}\n  method: put\n  operationId: updateCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customer_id}\n  method: delete\n  operationId: deleteCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customer_id}/bank_accounts\n\
  \  method: get\n  operationId: getBankAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customer_id}/bank_accounts/{bank_account_id}\n  method: get\n  operationId: getBankAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customer_id}/bank_accounts/{bank_account_id}/credit_analysis\n  method: get\n  operationId: getBankAccountCreditAnalysis\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customer_id}/bank_accounts/{bank_account_id}/credit_analysis/cashflow_insights\n  method: get\n  operationId: getBankAccountCreditAnalysisCashflowInsights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customer_id}/bank_accounts/{bank_account_id}/credit_analysis/expenditure_insights\n  method: get\n  operationId: getBankAccountCreditAnalysisExpenditureInsights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customer_id}/bank_accounts/{bank_account_id}/credit_analysis/income_insights\n  method: get\n  operationId: getBankAccountCreditAnalysisIncomeInsights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customer_id}/bank_accounts/{bank_account_id}/credit_analysis/loan_insights\n  method: get\n  operationId: getBankAccountCreditAnalysisLoanInsights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n\
  \    audit: none\n- path: /customers/{customer_id}/bank_accounts/{bank_account_id}/credit_analysis/risk_insights\n  method: get\n  operationId: getBankAccountCreditAnalysisRiskInsights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customer_id}/bank_accounts/{bank_account_id}/transactions\n  method: get\n  operationId: getBankAccountTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customer_id}/credit_analysis\n  method: get\n  operationId: getCustomerCreditAnalysis\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customer_id}/credit_analysis/cashflow_insights\n  method: get\n  operationId: getCustomerCreditAnalysisCashflowInsights\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customer_id}/credit_analysis/expenditure_insights\n  method: get\n  operationId: getCustomerCreditAnalysisExpenditureInsights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customer_id}/credit_analysis/income_insights\n  method: get\n  operationId: getCustomerCreditAnalysisIncomeInsights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customer_id}/credit_analysis/loan_insights\n  method: get\n  operationId: getCustomerCreditAnalysisLoanInsights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /customers/{customer_id}/credit_analysis/risk_insights\n  method: get\n  operationId: getCustomerCreditAnalysisRiskInsights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customer_id}/documents\n  method: post\n  operationId: uploadDocuments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customer_id}/documents\n  method: get\n  operationId: getDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customer_id}/documents/{document_id}\n  method: get\n  operationId: getDocumentResults\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customer_id}/documents/{document_id}\n  method: put\n  operationId: updateDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customer_id}/documents/{document_id}\n  method: delete\n  operationId: deleteDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customer_id}/open_banking_data\n  method: get\n  operationId: getOpenBankingData\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customer_id}/open_banking_data/inscribe_financial_data\n  method: post\n  operationId: uploadInscribeOpenBankingData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customer_id}/open_banking_data/mx_aggregated_data\n  method: post\n  operationId: uploadMXAggregatedOpenBankingData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customer_id}/open_banking_data/plaid_asset_report\n\
  \  method: post\n  operationId: uploadPlaidAssetReportOpenBankingData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customer_id}/open_banking_data/{open_banking_data_id}\n  method: delete\n  operationId: deleteOpenBankingData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customer_id}/plaid_assets\n  method: post\n  operationId: uploadPlaidAssetReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customer_id}/plaid_assets\n  method: get\n  operationId: getPlaidAssetReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{customer_id}/plaid_assets/{plaid_asset_report_id}\n  method: delete\n  operationId: deletePlaidAssetReport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{customer_id}/transactions\n  method: get\n  operationId: getCustomerTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /customers/{customer_id}/transactions/categories/{category}\n  method: patch\n  operationId: recategorizeTransactions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /health\n  method: get\n  operationId: reachability-check\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/categories\n  method: get\n  operationId: getTransactionCategories\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/inscribe/refs/heads/main/agentic-access/inscribe-agentic-access.yml
summary_line: 43 operations · 17 acting
tags:
- Fraud Prevention
- Document Verification
- Financial Services
- KYC
- KYB
- Bank Statements
- Paystubs
- Identity Verification
- Risk Management
- Fintech
- Artificial Intelligence
- Machine Learning
---
