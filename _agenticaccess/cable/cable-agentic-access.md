---
acting_count: 59
action_class_counts:
  acting: 59
  connected: 18
api_specs:
- filename: cable-alerts-api-openapi.yml
  format: yaml
  label: Cable alerts API
  slug: cable-alerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-alerts-api-openapi.yml
- filename: cable-authentication-api-openapi.yml
  format: yaml
  label: Cable authentication API
  slug: cable-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-authentication-api-openapi.yml
- filename: cable-business-api-openapi.yml
  format: yaml
  label: Cable business API
  slug: cable-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-business-api-openapi.yml
- filename: cable-checks-api-openapi.yml
  format: yaml
  label: Cable checks API
  slug: cable-checks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-checks-api-openapi.yml
- filename: cable-company-api-openapi.yml
  format: yaml
  label: Cable company API
  slug: cable-company-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-company-api-openapi.yml
- filename: cable-customersar-api-openapi.yml
  format: yaml
  label: Cable customerSar API
  slug: cable-customersar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-customersar-api-openapi.yml
- filename: cable-helper-api-openapi.yml
  format: yaml
  label: Cable helper API
  slug: cable-helper-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-helper-api-openapi.yml
- filename: cable-identityverification-api-openapi.yml
  format: yaml
  label: Cable identityVerification API
  slug: cable-identityverification-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-identityverification-api-openapi.yml
- filename: cable-onboardingflow-api-openapi.yml
  format: yaml
  label: Cable onboardingFlow API
  slug: cable-onboardingflow-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-onboardingflow-api-openapi.yml
- filename: cable-person-api-openapi.yml
  format: yaml
  label: Cable person API
  slug: cable-person-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-person-api-openapi.yml
- filename: cable-retail-api-openapi.yml
  format: yaml
  label: Cable retail API
  slug: cable-retail-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-retail-api-openapi.yml
- filename: cable-riskassessment-api-openapi.yml
  format: yaml
  label: Cable riskAssessment API
  slug: cable-riskassessment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-riskassessment-api-openapi.yml
- filename: cable-screening-api-openapi.yml
  format: yaml
  label: Cable screening API
  slug: cable-screening-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-screening-api-openapi.yml
- filename: cable-suspiciousactivities-api-openapi.yml
  format: yaml
  label: Cable suspiciousActivities API
  slug: cable-suspiciousactivities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-suspiciousactivities-api-openapi.yml
- filename: cable-transactionalerts-api-openapi.yml
  format: yaml
  label: Cable transactionAlerts API
  slug: cable-transactionalerts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-transactionalerts-api-openapi.yml
- filename: cable-transactionchecks-api-openapi.yml
  format: yaml
  label: Cable transactionChecks API
  slug: cable-transactionchecks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-transactionchecks-api-openapi.yml
- filename: cable-transactions-api-openapi.yml
  format: yaml
  label: Cable transactions API
  slug: cable-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-transactions-api-openapi.yml
- filename: cable-transactionsuspiciousactivities-api-openapi.yml
  format: yaml
  label: Cable transactionSuspiciousActivities API
  slug: cable-transactionsuspiciousactivities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-transactionsuspiciousactivities-api-openapi.yml
- filename: cable-upload-api-openapi.yml
  format: yaml
  label: Cable upload API
  slug: cable-upload-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-upload-api-openapi.yml
- filename: cable-utilities-api-openapi.yml
  format: yaml
  label: Cable utilities API
  slug: cable-utilities-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/openapi/cable-utilities-api-openapi.yml
consequence_counts:
  read: 18
  write: 59
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cable Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 77
overview: 'Cable exposes 77 API operations that an AI agent could call, of which 59 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 18 read and 59 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Cable
provider_slug: cable
slug: cable-agentic-access
source_filename: cable-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/cable-api-reference-openapi-original.yml, openapi/cable-customer-data-api-openapi-original.yml,\n  openapi/cable-transaction-data-api-openapi-original.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 77\n  by_action_class:\n    acting: 59\n    connected: 18\n  by_consequence:\n    write: 59\n    read: 18\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/auth/token\n  method: post\n  operationId: request-token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /v2/transaction\n  method: get\n  operationId: check-transaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/transaction\n  method: post\n  operationId: add-transaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/transaction\n  method: put\n  operationId: update-transaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/transaction\n  method: delete\n  operationId: delete-transaction\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/transactions/batch\n  method: post\n  operationId: add-transactions-batch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/transactions/batch\n  method: put\n  operationId: update-transactions-batch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /v2/transaction_check\n  method: get\n  operationId: check-transaction-check\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/transaction_check\n  method: post\n  operationId: add-transaction-check\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/transaction_check\n  method: put\n  operationId: update-transaction-checks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/transaction_alert\n  method:\
  \ get\n  operationId: check-transaction-alert\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/transaction_alert\n  method: post\n  operationId: add-transaction-alert\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/transaction_alert\n  method: put\n  operationId: update-transaction-alerts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/transaction_suspicious_activity\n  method: get\n  operationId: check-transaction-suspicious-activity\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/transaction_suspicious_activity\n  method: post\n  operationId: add-transaction-suspicious-activity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/transaction_suspicious_activity\n  method: put\n  operationId: update-transaction-suspicious-activities\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/screening\n  method: get\n  operationId: check-screening\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/screening\n  method: post\n  operationId: add-screening\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/screening\n  method: put\n  operationId: update-screenings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/risk_assessment\n  method: get\n  operationId: check-risk-assessment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/risk_assessment\n  method: post\n  operationId: add-risk-assessment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/risk_assessment\n  method: put\n  operationId: update-risk-assessments\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/person\n  method: get\n  operationId: check-person\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v2/person\n  method: post\n  operationId: add-person-info\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/person\n  method: put\n  operationId: update-persons\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/person\n  method: delete\n  operationId: delete-person\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      -\
  \ high-value\n    audit: required\n- path: /v2/identity_verification\n  method: get\n  operationId: check-identity-verification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/identity_verification\n  method: post\n  operationId: add-identity-verification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/identity_verification\n  method: put\n  operationId: update-identity-verifications\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n  \
  \  audit: required\n- path: /v2/onboarding_flow\n  method: get\n  operationId: check-onboarding-f-low\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/onboarding_flow\n  method: post\n  operationId: add-onboarding-flow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/onboarding_flow\n  method: put\n  operationId: update-onboarding-flows\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/company\n  method: get\n\
  \  operationId: check-company-info\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/company\n  method: post\n  operationId: add-company-info\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/company\n  method: put\n  operationId: update-companies\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/company\n  method: delete\n  operationId: delete-company\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/customer_sar\n  method: get\n  operationId: check-customer-sar\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/customer_sar\n  method: post\n  operationId: add-customer-sar\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/customer_sar\n  method: put\n  operationId: update-customer-sa-rs\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/deletion_request\n  method: get\n  operationId: get-deletion-request\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/upload/csv\n  method: post\n  operationId: upload-csv\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/retail/screening_check\n  method: post\n  operationId: v-1-retail-screening-check\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/retail/sar_info\n  method: post\n  operationId: v-1-retail-sar-info\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/retail/risk_assessment\n  method: post\n  operationId: v-1-retail-risk-assessment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/retail/person_info\n  method: post\n  operationId: v-1-retail-person-info\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/retail/onboarding_flow\n  method: post\n  operationId: v-1-retail-onboarding-flow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/retail/idv_info\n  method: post\n  operationId: v-1-retail-idv-info\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/retail/account_status\n  method: post\n  operationId: v-1-retail-account-status-info\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/retail/access_info\n  method: post\n  operationId: v-1-retail-access-info\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/business/screening_check\n  method: post\n  operationId: v-1-business-screening-check\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n  \
  \  audit: required\n- path: /v1/business/sar_info\n  method: post\n  operationId: v-1-business-sar-info\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/business/risk_assessment\n  method: post\n  operationId: v-1-business-risk-assessment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/business/person_info\n  method: post\n  operationId: v-1-business-person-info\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/business/onboarding_flow\n  method: post\n  operationId: v-1-business-onboarding-flow\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/business/idv_info\n  method: post\n  operationId: v-1-business-idv-info\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/business/company_info\n  method: post\n  operationId: v-1-business-company-info\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/business/account_status\n  method: post\n  operationId: v-1-business-account-status-info\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/business/access_info\n  method: post\n  operationId: v-1-business-access-info\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /status\n  method: get\n  operationId:\
  \ status-check\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /auth/token\n  method: post\n  operationId: request-token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction\n  method: get\n  operationId: check-transaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction\n  method: post\n  operationId: add-transaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction\n  method: put\n  operationId: update-transaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transactions/batch\n  method: post\n  operationId: add-transactions-batch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transactions/batch\n  method: put\n  operationId: update-transactions-batch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n     \
  \ max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction_check\n  method: get\n  operationId: check-transaction-check\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction_check\n  method: post\n  operationId: add-transaction-check\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction_check\n  method: put\n  operationId: update-transaction-check\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction_alert\n  method: get\n  operationId: check-transaction-alert\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction_alert\n  method: post\n  operationId: add-transaction-alert\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction_alert\n  method: put\n  operationId: update-transaction-alert\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /transaction_suspicious_activity\n  method: get\n  operationId: check-transaction-suspicious-activity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction_suspicious_activity\n  method: post\n  operationId: add-transaction-suspicious-activity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction_suspicious_activity\n  method: put\n  operationId: update-transaction-suspicious-activity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction_screening\n  method: get\n  operationId: check-transaction-screening\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transaction_screening\n  method: post\n  operationId: add-transaction-screening\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transaction_screening\n  method: put\n  operationId: update-transaction-screening\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cable/refs/heads/main/agentic-access/cable-agentic-access.yml
summary_line: 77 operations · 59 acting
tags:
- Company
- Compliance
- Financial Crime
- RegTech
- Anti-Money Laundering
- Transaction Monitoring
- Screening
- Risk Assessment
- Banking
- Fintech
---
