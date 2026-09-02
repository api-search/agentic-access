---
acting_count: 23
action_class_counts:
  acting: 23
api_specs:
- filename: 73-strings-asset-info-api-openapi.yml
  format: yaml
  label: 73 Strings Asset Info API
  slug: 73-strings-asset-info-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/73-strings/refs/heads/main/openapi/73-strings-asset-info-api-openapi.yml
- filename: 73-strings-captable-api-openapi.yml
  format: yaml
  label: 73 Strings Captable API
  slug: 73-strings-captable-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/73-strings/refs/heads/main/openapi/73-strings-captable-api-openapi.yml
- filename: 73-strings-documents-api-openapi.yml
  format: yaml
  label: 73 Strings Documents API
  slug: 73-strings-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/73-strings/refs/heads/main/openapi/73-strings-documents-api-openapi.yml
- filename: 73-strings-financial-data-api-openapi.yml
  format: yaml
  label: 73 Strings Financial Data API
  slug: 73-strings-financial-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/73-strings/refs/heads/main/openapi/73-strings-financial-data-api-openapi.yml
- filename: 73-strings-qualitative-data-api-openapi.yml
  format: yaml
  label: 73 Strings Qualitative Data API
  slug: 73-strings-qualitative-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/73-strings/refs/heads/main/openapi/73-strings-qualitative-data-api-openapi.yml
- filename: 73-strings-transaction-api-api-openapi.yml
  format: yaml
  label: 73 Strings Transaction API API
  slug: 73-strings-transaction-api-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/73-strings/refs/heads/main/openapi/73-strings-transaction-api-api-openapi.yml
consequence_counts:
  write: 23
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: 73 Strings Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 23
overview: '73 Strings exposes 23 API operations that an AI agent could call, of which 23 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 23 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: 73 Strings
provider_slug: 73-strings
slug: 73-strings-agentic-access
source_filename: 73-strings-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: generated\nsource: openapi/73-strings-asset-info-openapi.yml, openapi/73-strings-captable-openapi.yml,\n  openapi/73-strings-documents-openapi.yml, openapi/73-strings-financial-data-openapi.yml, openapi/73-strings-qualitative-data-openapi.yml,\n  openapi/73-strings-transaction-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    acting: 23\n  by_consequence:\n    write: 23\n  human_in_the_loop_required: 0\noperations:\n- path: /api/v1/ems/getEntityAttributeIds\n  method: post\n  operationId: getAttributeIDs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/ems/getEntityBusinessUnits\n  method: post\n  operationId: getEntityBusinessUnits\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/ems/getEntityList\n  method: post\n  operationId: getEntityList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/ems/getEntitySecuritiesList\n  method: post\n  operationId: getEntitySecuritiesList\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/version-list\n  method: post\n  operationId: getVersionList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/ems/captable/data\n  method: post\n  operationId: getCaptableData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/ems/getEntityDocumentDownloadFIle\n  method:\
  \ post\n  operationId: getDocumentDetailsByDocumentIDAndCompanyID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/ems/getEntityDocumentList\n  method: post\n  operationId: getDocumentIdForCompanyID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/data/getAllFinancialTexts\n  method: post\n  operationId: getAllFinancialTexts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/ems/entityBuFinancialData\n  method: post\n  operationId: entityBuFinancialData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/ems/entityFinancialData\n  method: post\n  operationId: entityFinancialData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/ems/entityFinancialData\n  method: post\n  operationId: streamEntityFinancialData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/ems/entitySecurityFinancialData\n  method: post\n  operationId: entitySecurityFinancialData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/ems/saveEntityFinancialData\n  method: post\n  operationId: companyFinancialData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/ems/customAttributeData\n\
  \  method: post\n  operationId: getCustomAttributeDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/ems/getEntityGeneralDetails\n  method: post\n  operationId: getGeneralDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/ems/getEntityQualitativeAnalysisData\n  method: post\n  operationId: getQualitativeAnalysisData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/unifiedTransaction\n  method: post\n  operationId: unifiedTransaction-v2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/unifiedTransaction\n  method: post\n  operationId: unifiedTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/transactionData\n  method: post\n  operationId: getTransactionData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/transactionType\n  method: post\n  operationId: getTransactionTypes\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/transactionVersion\n  method: post\n  operationId: getTransactionVersions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1/putfundTransactions\n  method: post\n  operationId: GTN_FUND_TRANSACTION\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/73-strings/refs/heads/main/agentic-access/73-strings-agentic-access.yml
summary_line: 23 operations · 23 acting
tags:
- Private Markets
- Valuation
- Portfolio Monitoring
- Private Equity
- Private Credit
- Venture Capital
- Alternative Assets
- Financial Data
- Data Extraction
- Fintech
- Asset Management
- Azure API Management
---
