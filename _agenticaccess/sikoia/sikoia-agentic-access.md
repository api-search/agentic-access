---
acting_count: 31
action_class_counts:
  acting: 31
  connected: 40
api_specs:
- filename: sikoia-adverse-media-api-openapi.yml
  format: yaml
  label: Sikoia Adverse Media API
  slug: sikoia-adverse-media-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/openapi/sikoia-adverse-media-api-openapi.yml
- filename: sikoia-affordability-insights-api-openapi.yml
  format: yaml
  label: Sikoia Affordability Insights API
  slug: sikoia-affordability-insights-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/openapi/sikoia-affordability-insights-api-openapi.yml
- filename: sikoia-authentication-api-openapi.yml
  format: yaml
  label: Sikoia Authentication API
  slug: sikoia-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/openapi/sikoia-authentication-api-openapi.yml
- filename: sikoia-banking-api-openapi.yml
  format: yaml
  label: Sikoia Banking API
  slug: sikoia-banking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/openapi/sikoia-banking-api-openapi.yml
- filename: sikoia-cases-api-openapi.yml
  format: yaml
  label: Sikoia Cases API
  slug: sikoia-cases-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/openapi/sikoia-cases-api-openapi.yml
- filename: sikoia-checklist-api-openapi.yml
  format: yaml
  label: Sikoia Checklist API
  slug: sikoia-checklist-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/openapi/sikoia-checklist-api-openapi.yml
- filename: sikoia-companies-people-api-openapi.yml
  format: yaml
  label: Sikoia Companies & People API
  slug: sikoia-companies-people-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/openapi/sikoia-companies-people-api-openapi.yml
- filename: sikoia-company-credit-report-api-openapi.yml
  format: yaml
  label: Sikoia Company Credit Report API
  slug: sikoia-company-credit-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/openapi/sikoia-company-credit-report-api-openapi.yml
- filename: sikoia-company-registry-api-openapi.yml
  format: yaml
  label: Sikoia Company Registry API
  slug: sikoia-company-registry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/openapi/sikoia-company-registry-api-openapi.yml
- filename: sikoia-data-sources-api-openapi.yml
  format: yaml
  label: Sikoia Data Sources API
  slug: sikoia-data-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/openapi/sikoia-data-sources-api-openapi.yml
- filename: sikoia-documents-api-openapi.yml
  format: yaml
  label: Sikoia Documents API
  slug: sikoia-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/openapi/sikoia-documents-api-openapi.yml
- filename: sikoia-excel-report-api-openapi.yml
  format: yaml
  label: Sikoia Excel Report API
  slug: sikoia-excel-report-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/openapi/sikoia-excel-report-api-openapi.yml
- filename: sikoia-identity-verification-api-openapi.yml
  format: yaml
  label: Sikoia Identity Verification API
  slug: sikoia-identity-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/openapi/sikoia-identity-verification-api-openapi.yml
- filename: sikoia-income-employer-verification-api-openapi.yml
  format: yaml
  label: Sikoia Income & Employer Verification API
  slug: sikoia-income-employer-verification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/openapi/sikoia-income-employer-verification-api-openapi.yml
- filename: sikoia-online-data-api-openapi.yml
  format: yaml
  label: Sikoia Online Data API
  slug: sikoia-online-data-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/openapi/sikoia-online-data-api-openapi.yml
- filename: sikoia-peps-sanctions-api-openapi.yml
  format: yaml
  label: Sikoia PEPs & Sanctions API
  slug: sikoia-peps-sanctions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/openapi/sikoia-peps-sanctions-api-openapi.yml
- filename: sikoia-user-management-api-openapi.yml
  format: yaml
  label: Sikoia User Management API
  slug: sikoia-user-management-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/openapi/sikoia-user-management-api-openapi.yml
- filename: sikoia-validation-checklists-api-openapi.yml
  format: yaml
  label: Sikoia Validation Checklists API
  slug: sikoia-validation-checklists-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/openapi/sikoia-validation-checklists-api-openapi.yml
- filename: sikoia-webhooks-api-openapi.yml
  format: yaml
  label: Sikoia Webhooks API
  slug: sikoia-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/openapi/sikoia-webhooks-api-openapi.yml
consequence_counts:
  read: 40
  write: 31
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Sikoia Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 71
overview: 'Sikoia exposes 71 API operations that an AI agent could call, of which 31 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 40 read and 31 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Sikoia
provider_slug: sikoia
slug: sikoia-agentic-access
source_filename: sikoia-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-21'\nmethod: generated\nsource: openapi/sikoia-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 71\n  by_action_class:\n    acting: 31\n    connected: 40\n  by_consequence:\n    write: 31\n    read: 40\n  human_in_the_loop_required: 0\noperations:\n- path: /token\n  method: post\n  operationId: POST_token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/users\n  method: get\n  operationId: GET_v2-users\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/webhooks\n  method: post\n  operationId: POST_v2-webhooks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/webhooks\n  method: get\n  operationId: GET_v2-webhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/webhooks/{webhook_id}\n  method: get\n  operationId: GET_v2-webhooks-webhook_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/webhooks/{webhook_id}\n  method: patch\n  operationId: PATCH_v2-webhooks-webhook_id\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/webhooks/{webhook_id}\n  method: delete\n  operationId: DELETE_v2-webhooks-webhook_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/webhooks/event-types\n  method: get\n  operationId: GET_v2-webhooks-event-types\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/webhooks/{webhook_id}/requests\n  method: get\n  operationId: GET_v2-webhooks-webhook_id-requests\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/webhooks/secrets\n  method: get\n  operationId: GET_v2-webhooks-secrets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/webhooks/secrets\n  method: post\n  operationId: POST_v2-webhooks-secrets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/webhooks/secrets\n  method: delete\n  operationId: DELETE_v2-webhooks-secrets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n   \
  \   triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/webhooks/secrets/rotate\n  method: patch\n  operationId: PATCH_v2-webhooks-secrets-rotate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/cases\n  method: get\n  operationId: GET_v2-cases\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/cases\n  method: post\n  operationId: POST_v2-cases\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v2/cases/{case_id}\n  method: get\n  operationId: GET_v2-cases-case_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/cases/{case_id}\n  method: patch\n  operationId: PATCH_v2-cases-case_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/cases/{case_id}\n  method: delete\n  operationId: DELETE_v2-cases-case_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/cases/{case_id}/entities\n  method:\
  \ post\n  operationId: POST_v2-cases-case_id-entities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/cases/{case_id}/entities\n  method: patch\n  operationId: PATCH_v2-cases-case_id-entities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/cases/{case_id}/entities/delete\n  method: post\n  operationId: POST_v2-cases-case_id-entities-delete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/company-registry-data\n  method: post\n  operationId: POST_v2-company-registry-data\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/companies/{company_id}/registry-data\n  method: get\n  operationId: GET_v2-companies-company_id-registry-data\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/company-registry-data/{request_id}\n  method: get\n  operationId: GET_v2-company-registry-data-request_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v2/company-registry-data/picklist\n  method: post\n  operationId: POST_v2-company-registry-data-picklist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/company-registry-data/search\n  method: post\n  operationId: POST_v2-company-registry-data-search\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/company-credit-reports\n  method: post\n  operationId: POST_v2-company-credit-reports\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/companies/{company_id}/credit-reports\n  method: get\n  operationId: GET_v2-companies-company_id-credit-reports\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/company-credit-reports/{request_id}\n  method: get\n  operationId: GET_v2-company-credit-reports-request_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/company-credit-reports/picklist\n  method: post\n  operationId: POST_v2-company-credit-reports-picklist\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/openbanking\n  method: post\n  operationId: POST_v2-openbanking\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/openbanking/{bank_connection_id}\n  method: get\n  operationId: GET_v2-openbanking-bank_connection_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/openbanking/{bank_connection_id}\n  method: delete\n  operationId: DELETE_v2-openbanking-bank_connection_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/{entity_type}/{entity_id}/openbanking\n  method: get\n  operationId: GET_v2-entity_type-entity_id-openbanking\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/bankaccounts/{account_connection_id}\n  method: get\n  operationId: GET_v2-bankaccounts-account_connection_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/{entity_type}/{entity_id}/bankaccounts\n  method: get\n  operationId: GET_v2-entity_type-entity_id-bankaccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/bankaccounts/{account_connection_id}/balances\n  method: get\n  operationId: GET_v2-bankaccounts-account_connection_id-balances\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/bankaccounts/{account_connection_id}/transactions\n  method: get\n  operationId: GET_v2-bankaccounts-account_connection_id-transactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/bankaccounts/{account_connection_id}/refresh\n  method: post\n  operationId: POST_v2-bankaccounts-account_connection_id-refresh\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/peps-sanctions\n  method: post\n  operationId: POST_v2-peps-sanctions\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/{entity_type}/{entity_id}/peps-sanctions\n  method: get\n  operationId: GET_v2-entity_type-entity_id-peps-sanctions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/adverse-media\n  method: post\n  operationId: POST_v2-adverse-media\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/{entity_type}/{entity_id}/adverse-media\n  method: get\n  operationId: GET_v2-entity_type-entity_id-adverse-media\n  x-agentic-access:\n   \
  \ action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/documents\n  method: post\n  operationId: POST_v2-documents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/documents/{document_id}\n  method: get\n  operationId: GET_v2-documents-document_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/documents/{document_id}\n  method: delete\n  operationId: DELETE_v2-documents-document_id\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/{entity_type}/{entity_id}/documents\n  method: get\n  operationId: GET_v2-entity_type-entity_id-documents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/{entity_type}/{entity_id}/integrity-checks\n  method: get\n  operationId: GET_v2-entity_type-entity_id-integrity-checks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/documents/{document_id}/integrity-checks\n  method: get\n  operationId: GET_v2-documents-document_id-integrity-checks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/identity\n  method: post\n  operationId: POST_v2-identity\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/persons/{person_id}/identity-verifications\n  method: get\n  operationId: GET_v2-persons-person_id-identity-verifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/identity/{request_id}\n  method: get\n  operationId: GET_v2-identity-request_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/company-online-data\n  method: post\n  operationId: POST_v2-company-online-data\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n   \
  \   max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/companies/{company_id}/online-data\n  method: get\n  operationId: GET_v2-companies-company_id-online-data\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/company-online-data/{request_id}\n  method: get\n  operationId: GET_v2-company-online-data-request_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/affordability-insights\n  method: post\n  operationId: POST_v2-affordability-insights\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /v2/{entity_type}/{entity_id}/affordability-insights\n  method: get\n  operationId: GET_v2-entity_type-entity_id-affordability-insights\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/affordability-insights/{request_id}\n  method: get\n  operationId: GET_v2-affordability-insights-request_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/affordability-insights/{request_id}/transactions\n  method: get\n  operationId: GET_v2-affordability-insights-request_id-transactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/affordability-insights/{request_id}/transaction-details\n  method: get\n  operationId:\
  \ GET_v2-affordability-insights-request_id-transaction-details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/income-employer\n  method: post\n  operationId: POST_v2-income-employer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/{entity_type}/{entity_id}/income-employer\n  method: get\n  operationId: GET_v2-entity_type-entity_id-incomeemployer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/income-employer/{request_id}\n  method: get\n  operationId: GET_v2-income-employer-request_id\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/income-employer/{request_id}/additional-details\n  method: get\n  operationId: GET_v2-income-employer-request_id-additional-details\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/{entity_type}/{entity_id}/insight-data-sources\n  method: get\n  operationId: GET_v2-entity_type-entity_id-insight-data-sources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/validation-checks/validation-types\n  method: get\n  operationId: GET_v2-validation-checks-validation-types\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/validation-checks\n  method: post\n  operationId:\
  \ POST_v2-validation-checks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/{entity_type}/{entity_id}/validation-checks\n  method: get\n  operationId: GET_v2-entity_type-entity_id-validation-checks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/validation-checks/{validation_instance_id}\n  method: get\n  operationId: GET_v2-validation-checks-validation_instance_id\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/{entity_type}/{entity_id}/excel-report\n  method: get\n  operationId: GET_v2-entity_type-entity_id-excel-report\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/completeness-income-checks\n  method: post\n  operationId: POST_v2-completeness-income-checks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/sikoia/refs/heads/main/agentic-access/sikoia-agentic-access.yml
summary_line: 71 operations · 31 acting
tags:
- Company
- Financial Services
- Identity Verification
- KYC
- KYB
- Onboarding
- Open Banking
- Credit
- Affordability
- Fraud & AML
- Document Verification
- RegTech
---
