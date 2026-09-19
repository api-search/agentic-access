---
acting_count: 11
action_class_counts:
  acting: 11
  connected: 50
api_specs:
- filename: orbii-business-category-assignment-api-openapi.yml
  format: yaml
  label: Orbii Business Category Assignment API
  slug: orbii-business-category-assignment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-business-category-assignment-api-openapi.yml
- filename: orbii-categories-api-openapi.yml
  format: yaml
  label: Orbii Categories API
  slug: orbii-categories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-categories-api-openapi.yml
- filename: orbii-clients-api-openapi.yml
  format: yaml
  label: Orbii Clients API
  slug: orbii-clients-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-clients-api-openapi.yml
- filename: orbii-company-management-api-openapi.yml
  format: yaml
  label: Orbii Company Management API
  slug: orbii-company-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-company-management-api-openapi.yml
- filename: orbii-data-check-api-openapi.yml
  format: yaml
  label: Orbii Data Check API
  slug: orbii-data-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-data-check-api-openapi.yml
- filename: orbii-general-api-openapi.yml
  format: yaml
  label: Orbii General API
  slug: orbii-general-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-general-api-openapi.yml
- filename: orbii-invoices-api-openapi.yml
  format: yaml
  label: Orbii Invoices API
  slug: orbii-invoices-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-invoices-api-openapi.yml
- filename: orbii-kpis-api-openapi.yml
  format: yaml
  label: Orbii KPIs API
  slug: orbii-kpis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-kpis-api-openapi.yml
- filename: orbii-lending-actions-api-openapi.yml
  format: yaml
  label: Orbii Lending Actions API
  slug: orbii-lending-actions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-lending-actions-api-openapi.yml
- filename: orbii-merchants-api-openapi.yml
  format: yaml
  label: Orbii Merchants API
  slug: orbii-merchants-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-merchants-api-openapi.yml
- filename: orbii-risk-assessment-api-openapi.yml
  format: yaml
  label: Orbii Risk Assessment API
  slug: orbii-risk-assessment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-risk-assessment-api-openapi.yml
- filename: orbii-subcategories-api-openapi.yml
  format: yaml
  label: Orbii Subcategories API
  slug: orbii-subcategories-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-subcategories-api-openapi.yml
- filename: orbii-transactions-api-openapi.yml
  format: yaml
  label: Orbii Transactions API
  slug: orbii-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-transactions-api-openapi.yml
- filename: orbii-ibans-api-openapi.yml
  format: yaml
  label: Orbii IBA Ns API
  slug: orbii-ibans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-ibans-api-openapi.yml
- filename: orbii-pdfs-api-openapi.yml
  format: yaml
  label: Orbii PD Fs API
  slug: orbii-pdfs-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/openapi/orbii-pdfs-api-openapi.yml
consequence_counts:
  physical: 4
  read: 50
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Orbii Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /categorise-cheque-deposits
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /categorise-partner-transactions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoice-extract-upload
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /start-invoice-extraction
operation_count: 61
overview: 'Orbii exposes 61 API operations that an AI agent could call, of which 11 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 50 read, 7 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Orbii
provider_slug: orbii
slug: orbii-agentic-access
source_filename: orbii-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/orbii-business-category-assignment-api-openapi.yml, openapi/orbii-categories-api-openapi.yml,\n  openapi/orbii-clients-api-openapi.yml, openapi/orbii-company-management-api-openapi.yml, openapi/orbii-data-check-api-openapi.yml,\n  openapi/orbii-general-api-openapi.yml, openapi/orbii-ibans-api-openapi.yml, openapi/orbii-invoices-api-openapi.yml,\n  openapi/orbii-kpis-api-openapi.yml, openapi/orbii-lending-actions-api-openapi.yml, openapi/orbii-merchants-api-openapi.yml,\n  openapi/orbii-pdfs-api-openapi.yml, openapi/orbii-risk-assessment-api-openapi.yml, openapi/orbii-subcategories-api-openapi.yml,\n  openapi/orbii-transactions-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations:\
  \ 61\n  by_action_class:\n    connected: 50\n    acting: 11\n  by_consequence:\n    read: 50\n    write: 7\n    physical: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /assign-category\n  method: get\n  operationId: getAssignCategory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assign-category\n  method: post\n  operationId: postAssignCategory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /categories/{clientname}\n  method: get\n  operationId: getCategoriesByClientname\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clients\n\
  \  method: get\n  operationId: getClients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clients/range\n  method: get\n  operationId: getClientsRange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /add-company\n  method: post\n  operationId: postAddCompany\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Check-for-new-data-received\n  method: get\n  operationId: getCheckForNewDataReceived\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /\n  method: get\n  operationId: getRoot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /ibans\n  method: get\n  operationId: getIbans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoice-extract-upload\n  method: post\n  operationId: postInvoiceExtractUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /start-invoice-extraction\n  method: post\n  operationId: postStartInvoiceExtraction\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /invoice-kpis/customer/{customer_id}\n  method: get\n  operationId: getInvoiceKpisCustomerByCustomerId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoice-risk_assessment/customer/{customer_id}\n  method: get\n  operationId: getInvoiceRiskAssessmentCustomerByCustomerId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoice-band_classification/customer/{customer_id}\n  method: get\n  operationId: getInvoiceBandClassificationCustomerByCustomerId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoice-company-kpis/customer/{customer_id}\n  method: get\n  operationId: getInvoiceCompanyKpisCustomerByCustomerId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoice-company-risk_assessment/customer/{customer_id}\n  method: get\n  operationId: getInvoiceCompanyRiskAssessmentCustomerByCustomerId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoice-company-band_classification/customer/{customer_id}\n  method: get\n  operationId: getInvoiceCompanyBandClassificationCustomerByCustomerId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoice-suggested-loan/customer/{customer_id}\n  method: get\n\
  \  operationId: getInvoiceSuggestedLoanCustomerByCustomerId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoice-suggested-loan-allocation/customer/{customer_id}\n  method: get\n  operationId: getInvoiceSuggestedLoanAllocationCustomerByCustomerId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /invoice-suggested-loan-summary/customer/{customer_id}\n  method: get\n  operationId: getInvoiceSuggestedLoanSummaryCustomerByCustomerId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client-kpis/customer/{customer_id}\n  method: get\n  operationId: getClientKpisCustomerByCustomerId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /predictive-kpis/customer/{customer_id}\n  method: get\n  operationId: getPredictiveKpisCustomerByCustomerId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client-kpis\n  method: get\n  operationId: getClientKpis\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client-kpis/{clientname}\n  method: get\n  operationId: getClientKpisByClientname\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /predictive-kpis\n  method: get\n  operationId: getPredictiveKpis\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /predictive-kpis/{clientname}\n\
  \  method: get\n  operationId: getPredictiveKpisByClientname\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /log-lending\n  method: post\n  operationId: postLogLending\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transactions_with_merchant/customer/{customer_id}\n  method: get\n  operationId: getTransactionsWithMerchantCustomerByCustomerId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paged-transactions_with_merchant/customer/{customer_id}\n  method: get\n  operationId: getPagedTransactionsWithMerchantCustomerByCustomerId\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /top_buyers/customer/{customer_id}\n  method: get\n  operationId: getTopBuyersCustomerByCustomerId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /top_sellers/customer/{customer_id}\n  method: get\n  operationId: getTopSellersCustomerByCustomerId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /top_buyers_recent/customer/{customer_id}\n  method: get\n  operationId: getTopBuyersRecentCustomerByCustomerId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /top_sellers_recent/customer/{customer_id}\n  method: get\n  operationId: getTopSellersRecentCustomerByCustomerId\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions_with_merchant/customer/{customer_id}/range\n  method: get\n  operationId: getTransactionsWithMerchantCustomerByCustomerIdRange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paged-transactions_with_merchant/customer/{customer_id}/range\n  method: get\n  operationId: getPagedTransactionsWithMerchantCustomerByCustomerIdRange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pdf-list\n  method: get\n  operationId: getPdfList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pdf-list-from-date\n  method: get\n\
  \  operationId: getPdfListFromDate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pdf-upload\n  method: post\n  operationId: postPdfUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /start-pdf-extraction\n  method: post\n  operationId: postStartPdfExtraction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /risk_assessment/customer/{customer_id}\n  method: get\n  operationId: getRiskAssessmentCustomerByCustomerId\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /band_classification/customer/{customer_id}\n  method: get\n  operationId: getBandClassificationCustomerByCustomerId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /update-kpi-rule\n  method: post\n  operationId: postUpdateKpiRule\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rerun-assessment\n  method: post\n  operationId: postRerunAssessment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /band_classification\n  method: get\n  operationId: getBandClassification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /subcategories/{clientname}\n  method: get\n  operationId: getSubcategoriesByClientname\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions\n  method: get\n  operationId: getTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/customer/{customer_id}\n  method: get\n  operationId: getTransactionsCustomerByCustomerId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/date/{date}\n  method: get\n  operationId: getTransactionsDateByDate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/daterange\n  method: get\n  operationId: getTransactionsDaterange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/range\n  method: get\n  operationId: getTransactionsRange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/{clientname}\n  method: get\n  operationId: getTransactionsByClientname\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n- path: /transactions/{clientname}/date/{date}\n  method: get\n  operationId: getTransactionsByClientnameDateByDate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/{clientname}/daterange\n  method: get\n  operationId: getTransactionsByClientnameDaterange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/{clientname}/range\n  method: get\n  operationId: getTransactionsByClientnameRange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/iban/{iban}\n  method: get\n  operationId: getTransactionsIbanByIban\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /paged-transactions/customer/{customer_id}\n  method: get\n  operationId: getPagedTransactionsCustomerByCustomerId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paged-transactions/{clientname}\n  method: get\n  operationId: getPagedTransactionsByClientname\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /categorise-cheque-deposits\n  method: post\n  operationId: postCategoriseChequeDeposits\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /categorise-partner-transactions\n\
  \  method: post\n  operationId: postCategorisePartnerTransactions\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transactions/customer/{customer_id}/range\n  method: get\n  operationId: getTransactionsCustomerByCustomerIdRange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paged-transactions/customer/{customer_id}/range\n  method: get\n  operationId: getPagedTransactionsCustomerByCustomerIdRange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/orbii/refs/heads/main/agentic-access/orbii-agentic-access.yml
summary_line: 61 operations · 11 acting
tags:
- Company
- Artificial Intelligence
- Lending
- Credit
- Fintech
- Underwriting
- Banking
- SME
- Embedded Finance
- MENA
- Risk
---
