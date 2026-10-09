---
acting_count: 19
action_class_counts:
  acting: 19
  connected: 20
api_specs:
- filename: spliceforms-account-data-inquiry-api-openapi.yml
  format: yaml
  label: Spliceforms account data inquiry API
  slug: spliceforms-account-data-inquiry-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spliceforms/refs/heads/main/openapi/spliceforms-account-data-inquiry-api-openapi.yml
- filename: spliceforms-branches-api-openapi.yml
  format: yaml
  label: Spliceforms Branches API
  slug: spliceforms-branches-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spliceforms/refs/heads/main/openapi/spliceforms-branches-api-openapi.yml
- filename: spliceforms-calculators-api-openapi.yml
  format: yaml
  label: Spliceforms Calculators API
  slug: spliceforms-calculators-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spliceforms/refs/heads/main/openapi/spliceforms-calculators-api-openapi.yml
- filename: spliceforms-codesets-api-openapi.yml
  format: yaml
  label: Spliceforms Codesets API
  slug: spliceforms-codesets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spliceforms/refs/heads/main/openapi/spliceforms-codesets-api-openapi.yml
- filename: spliceforms-consents-api-openapi.yml
  format: yaml
  label: Spliceforms Consents API
  slug: spliceforms-consents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spliceforms/refs/heads/main/openapi/spliceforms-consents-api-openapi.yml
- filename: spliceforms-data-validations-api-openapi.yml
  format: yaml
  label: Spliceforms data validations API
  slug: spliceforms-data-validations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spliceforms/refs/heads/main/openapi/spliceforms-data-validations-api-openapi.yml
- filename: spliceforms-form-capture-api-openapi.yml
  format: yaml
  label: Spliceforms Form Capture API
  slug: spliceforms-form-capture-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spliceforms/refs/heads/main/openapi/spliceforms-form-capture-api-openapi.yml
- filename: spliceforms-location-api-openapi.yml
  format: yaml
  label: Spliceforms Location API
  slug: spliceforms-location-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spliceforms/refs/heads/main/openapi/spliceforms-location-api-openapi.yml
- filename: spliceforms-otp-auth-api-openapi.yml
  format: yaml
  label: Spliceforms OTP Auth API
  slug: spliceforms-otp-auth-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spliceforms/refs/heads/main/openapi/spliceforms-otp-auth-api-openapi.yml
- filename: spliceforms-status-tracking-api-openapi.yml
  format: yaml
  label: Spliceforms Status Tracking API
  slug: spliceforms-status-tracking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spliceforms/refs/heads/main/openapi/spliceforms-status-tracking-api-openapi.yml
- filename: spliceforms-submission-api-openapi.yml
  format: yaml
  label: Spliceforms Submission API
  slug: spliceforms-submission-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spliceforms/refs/heads/main/openapi/spliceforms-submission-api-openapi.yml
consequence_counts:
  physical: 1
  read: 20
  write: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Spliceforms Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/otp/resend
operation_count: 39
overview: 'Spliceforms exposes 39 API operations that an AI agent could call, of which 19 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 20 read, 18 write, and 1 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Spliceforms
provider_slug: spliceforms
slug: spliceforms-agentic-access
source_filename: spliceforms-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: generated\nsource: openapi/spliceforms-auth-services-openapi.yml, openapi/spliceforms-capture-services-openapi.yml,\n  openapi/spliceforms-data-services-openapi.yml, openapi/spliceforms-inquiry-services-openapi.yml,\n  openapi/spliceforms-processing-service-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 39\n  by_action_class:\n    acting: 19\n    connected: 20\n  by_consequence:\n    write: 18\n    physical: 1\n    read: 20\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/otp/initiate\n  method: post\n  operationId: initiateAuthentication\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/otp/resend\n  method: post\n  operationId: resendOTP\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/otp/token\n  method: post\n  operationId: verifyOTPAndIssueToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/application-forms\n  method: post\n  operationId: initiateApplication\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/application-forms/{applicationId}/accounts\n  method: post\n  operationId: saveAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/application-forms/{applicationId}/accounts/{accountSerialNo}\n  method: get\n  operationId: fetchAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/application-forms/{applicationId}/accounts/{accountSerialNo}/nomination\n  method: post\n  operationId: saveAccountNomination\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/application-forms/{applicationId}/accounts/{accountSerialNo}/nomination\n  method: get\n  operationId: fetchAccountNomination\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/application-forms/{applicationId}/accounts/{accountSerialNo}/nomination\n  method: delete\n  operationId: deleteAccountNomination\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/application-forms/{applicationId}/payin-preferences\n\
  \  method: post\n  operationId: savePayinPreferences\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/application-forms/{applicationId}/payin-preferences\n  method: get\n  operationId: fetchPayinPreferences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/application-forms/{applicationId}/payin-preferences\n  method: delete\n  operationId: deletePayinPreferences\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v1/application-forms/{applicationId}/staff\n  method: post\n  operationId: saveStaff\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/application-forms/{applicationId}/staff\n  method: get\n  operationId: fetchStaff\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/application-forms/{applicationId}/staff\n  method: delete\n  operationId: deleteStaff\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/application-forms/{applicationId}/consents\n\
  \  method: post\n  operationId: saveConsents\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/application-forms/{applicationId}/consents\n  method: get\n  operationId: fetchConsents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/application-forms/{applicationId}/payin\n  method: post\n  operationId: initiatePayin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/application-forms/{applicationId}/payin/status\n\
  \  method: post\n  operationId: fetchPayinStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/application-forms/{applicationId}/validation\n  method: post\n  operationId: validateApplicationForm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/application-forms/{applicationId}/submission\n  method: post\n  operationId: submitApplicationForm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/applications/{applicationId}/status\n\
  \  method: get\n  operationId: fetchApplicationStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/branches\n  method: get\n  operationId: fetchBranches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/branches/states\n  method: get\n  operationId: fetchBranchStates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/branches/cities\n  method: get\n  operationId: fetchBranchCities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/branches/districts\n  method: get\n  operationId: fetchBranchDistricts\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/consent-definitions\n  method: get\n  operationId: fetchConsentDefinitions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/states\n  method: get\n  operationId: fetchStates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/cities\n  method: get\n  operationId: fetchCities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/codesets\n  method: get\n  operationId: fetchCodesets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/codesets/{codeset}\n  method:\
  \ get\n  operationId: get-v1-data-codesets-codes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/banks\n  method: get\n  operationId: get-v1-banks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/banks/branches\n  method: get\n  operationId: get-v1-banks-branches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customer/vpa/verification\n  method: post\n  operationId: verifyCustomerVpa\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n-\
  \ path: /v1/customer/bank-account/verification\n  method: post\n  operationId: verifyCustomerBankAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/customer/accounts/nominees/get\n  method: post\n  operationId: getCustomerAccountNominees\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customer/fd-maturity\n  method: post\n  operationId: calculateFDMaturity\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v1/applications/submit\n  method: post\n  operationId: submitApplicationForm\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/applications/status\n  method: post\n  operationId: get-v1-applications-status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spliceforms/refs/heads/main/agentic-access/spliceforms-agentic-access.yml
summary_line: 39 operations · 19 acting
tags:
- Company
- API Banking
- Open Banking
- Embedded Banking
- Fintech
- Developer Portal
- Banking
- India
---
