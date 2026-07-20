---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 14
api_specs:
- filename: credilinqai-openapi.yml
  format: yaml
  label: CrediLinq API
  slug: credilinq-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/credilinqai/refs/heads/main/openapi/credilinqai-openapi.yml
consequence_counts:
  read: 14
  safety-critical: 17
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 17
kind: agentic-access
layout: agentic-access
method: generated
name: Credilinqai Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/auth/generate-token
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/kyc/individual/create
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/kyc/individual/update
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/kyc/send-for-review
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/loan
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/loan/calculateloanschedule
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/loan/disburse
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/onboarding/check-eligibility
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/onboarding/initiate-data-processing
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/onboarding/send-agreement
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/payments/loan/initiate-payment
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/payments/loan/make-payment
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/payments/loans/reconcilepayment
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/kyc/customer/create
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v2/kyc/customer/update
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v2/kyc/director/create
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v2/kyc/director/update
operation_count: 31
overview: 'Credilinq.ai exposes 31 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 14 read and 17 safety-critical.


  17 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Credilinq.ai
provider_slug: credilinqai
slug: credilinqai-agentic-access
source_filename: credilinqai-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-18'\nmethod: generated\nsource: openapi/credilinqai-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 31\n  by_action_class:\n    acting: 17\n    connected: 14\n  by_consequence:\n    safety-critical: 17\n    read: 14\n  human_in_the_loop_required: 17\noperations:\n- path: /v1/auth/generate-token\n  method: post\n  operationId: AuthenticationController_generateToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/onboarding/check-eligibility\n\
  \  method: post\n  operationId: OnboardingController_initiateOnboardingApplication\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/onboarding/initiate-data-processing\n  method: post\n  operationId: OnboardingController_initiateDaraProcessing\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/onboarding/send-agreement\n  method: post\n  operationId: OnboardingController_generateKycDocusign\n  x-agentic-access:\n    action-class: acting\n   \
  \ consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/kyc/customer/create\n  method: post\n  operationId: KycController_createCustomerKYCV2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/kyc/customer/update\n  method: put\n  operationId: KycController_updateCustomerKYCV2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/kyc/director/create\n  method: post\n  operationId: KycController_addDirectorKycV2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v2/kyc/director/update\n  method: put\n  operationId: KycController_updateDirectorInformationV2\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/kyc/send-for-review\n  method: post\n  operationId: KycController_sendKycForReview\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/kyc/details/{applicationId}\n  method: get\n  operationId: KycController_getKycData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/kyc/individual/create\n  method: post\n  operationId: KycController_createIndividualCustomerKYC\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/kyc/individual/update\n\
  \  method: put\n  operationId: KycController_updateIndividualCustomerKYC\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/customer/{customerReferenceNo}/payment-methods\n  method: get\n  operationId: ClientController_getCustomerChosenPaymentMethods\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customer/{customerReferenceNo}/line-details\n  method: get\n  operationId: ClientController_getCustomerCreditLineDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customer/{customerReferenceNo}/loans\n\
  \  method: get\n  operationId: ClientController_getCustomerActiveLoans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/customer/holidays/{customerReferenceNo}\n  method: get\n  operationId: ClientController_getHolidaysByCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/loan/calculateloanschedule\n  method: post\n  operationId: DrawdownController_calculateRepaymentScheduleBNPL\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/loan\n  method: post\n  operationId: DrawdownController_createDrawdownBNPL\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/loan/disburse\n  method: post\n  operationId: DrawdownController_disburseDrawdownBNPL\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/loan/summary/{loanId}\n  method: get\n  operationId: DrawdownController_getDrawdownBNPL\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payments/loan/initiate-payment\n\
  \  method: post\n  operationId: PaymentsController_initiatePaymentBNPLV1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/payments/loan/make-payment\n  method: post\n  operationId: PaymentsController_makePaymentBNPLV1\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/payments/loans/reconcilepayment\n  method: post\n  operationId: PaymentsController_verifyPaymentBNPL\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/payments/loans/payment/{loanId}\n  method: get\n  operationId: PaymentsController_getAllPaymentsV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reports/partner/partner-report\n  method: get\n  operationId: ReportController_getPartnerReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/reports/customer/{customerReferenceNo}/dashboard\n  method: get\n  operationId: ReportController_getClientDashboardData\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v1/reports/credit-history/{customerReferenceNo}\n  method: get\n  operationId: ReportController_GetAllCreditHistoryByRefNo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/others/demographic-info/postal-codes\n  method: get\n  operationId: OthersController_getPostalCodes\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/others/demographic-info/countries\n  method: get\n  operationId: OthersController_getCountries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/others/demographic-info/addresses\n  method: get\n  operationId: OthersController_getFullAddresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/others/kyc/document-types\n  method: get\n  operationId: OthersController_getKycDocumentType\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/credilinqai/refs/heads/main/agentic-access/credilinqai-agentic-access.yml
summary_line: 31 operations · 17 acting · 17 human-in-the-loop
tags:
- Company
- Fintech
- Embedded Finance
- Lending
- BNPL
- Credit
- Payments
- KYC
- B2B
---
