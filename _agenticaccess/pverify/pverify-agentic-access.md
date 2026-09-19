---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 21
api_specs:
- filename: pverify-authentication-api-openapi.yml
  format: yaml
  label: pVerify Authentication API
  slug: pverify-authentication-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-authentication-api-openapi.yml
- filename: pverify-eligibility-api-openapi.yml
  format: yaml
  label: pVerify Eligibility API
  slug: pverify-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-eligibility-api-openapi.yml
- filename: pverify-dental-eligibility-api-openapi.yml
  format: yaml
  label: pVerify Dental Eligibility API
  slug: pverify-dental-eligibility-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-dental-eligibility-api-openapi.yml
- filename: pverify-insurance-discovery-api-openapi.yml
  format: yaml
  label: pVerify Insurance Discovery API
  slug: pverify-insurance-discovery-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-insurance-discovery-api-openapi.yml
- filename: pverify-mbi-lookup-api-openapi.yml
  format: yaml
  label: pVerify MBI Lookup API
  slug: pverify-mbi-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-mbi-lookup-api-openapi.yml
- filename: pverify-patient-demographic-validator-api-openapi.yml
  format: yaml
  label: pVerify Patient Demographic Validator API
  slug: pverify-patient-demographic-validator-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-patient-demographic-validator-api-openapi.yml
- filename: pverify-claim-status-api-openapi.yml
  format: yaml
  label: pVerify Claim Status API
  slug: pverify-claim-status-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-claim-status-api-openapi.yml
- filename: pverify-estimation-api-openapi.yml
  format: yaml
  label: pVerify Patient Cost Estimator API
  slug: pverify-estimation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-estimation-api-openapi.yml
- filename: pverify-payers-api-openapi.yml
  format: yaml
  label: pVerify Payers API
  slug: pverify-payers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-payers-api-openapi.yml
- filename: pverify-cgx-widget-api-openapi.yml
  format: yaml
  label: pVerify CGX Widget API
  slug: pverify-cgx-widget-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-cgx-widget-api-openapi.yml
- filename: pverify-same-or-similar-api-openapi.yml
  format: yaml
  label: pVerify Same or Similar API (discontinued)
  slug: pverify-same-or-similar-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-same-or-similar-api-openapi.yml
- filename: pverify-cmn-api-openapi.yml
  format: yaml
  label: pVerify CMN API (discontinued)
  slug: pverify-cmn-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-cmn-api-openapi.yml
- filename: pverify-snf-api-openapi.yml
  format: yaml
  label: pVerify SNF API (discontinued)
  slug: pverify-snf-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/openapi/pverify-snf-api-openapi.yml
consequence_counts:
  read: 21
  write: 18
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Pverify Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 39
overview: 'pVerify exposes 39 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 21 read and 18 write.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: pVerify
provider_slug: pverify
slug: pverify-agentic-access
source_filename: pverify-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-16'\nmethod: generated\nsource: openapi/pverify-authentication-api-openapi.yml, openapi/pverify-cgx-widget-api-openapi.yml,\n  openapi/pverify-claim-status-api-openapi.yml, openapi/pverify-cmn-api-openapi.yml, openapi/pverify-dental-eligibility-api-openapi.yml,\n  openapi/pverify-eligibility-api-openapi.yml, openapi/pverify-estimation-api-openapi.yml, openapi/pverify-insurance-discovery-api-openapi.yml,\n  openapi/pverify-mbi-lookup-api-openapi.yml, openapi/pverify-patient-demographic-validator-api-openapi.yml,\n  openapi/pverify-payers-api-openapi.yml, openapi/pverify-same-or-similar-api-openapi.yml, openapi/pverify-snf-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 39\n  by_action_class:\n    acting: 18\n\
  \    connected: 21\n  by_consequence:\n    write: 18\n    read: 21\n  human_in_the_loop_required: 0\noperations:\n- path: /Token\n  method: post\n  operationId: createToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Widget/Setup\n  method: post\n  operationId: createWidgetSetup\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/CGXInquiry\n  method: post\n  operationId: cgxInquiry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n    \
  \  max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /API/ClaimStatusInquiry\n  method: post\n  operationId: claimStatusInquiry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /API/GetClaimStatusResponse/{requestId}\n  method: get\n  operationId: getClaimStatusResponse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /API/CMNInquiry\n  method: post\n  operationId: cmnInquiry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /API/GetCMNResponse/{requestId}\n  method: get\n  operationId: getCMNResponse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /PDFReport/CMN/{id}\n  method: get\n  operationId: getCmnReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /API/GetEligibilitySummary/{requestId}\n  method: get\n  operationId: getEligibilitySummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/DentalEligibilitySummary\n  method: post\n  operationId: dentalEligibilitySummary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/DentalEligibilityBenefitSummary\n  method: post\n  operationId: dentalEligibilityBenefitSummary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v2/DentalEligibilitySummary\n  method: post\n  operationId: dentalEligibilitySummaryV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /API/GetDentalEligibilitySummary/{requestId}\n  method: get\n \
  \ operationId: getDentalEligibilitySummary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/EligibilitySummary\n  method: post\n  operationId: eligibilitySummary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /API/GetEligibility271/{requestId}\n  method: get\n  operationId: getEligibility271\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /API/EasyEligibilitySummary\n  method: post\n  operationId: easyEligibilitySummary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n   \
  \ token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /API/GetPendingInquiries\n  method: get\n  operationId: getPendingInquiries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /API/CancelTransaction\n  method: post\n  operationId: cancelTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /Report/EligibilityPDFReport/{requestId}\n  method: get\n  operationId: getEligibilityPdfReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /API/GetEligibilityDetailsURL/{requestId}\n  method: get\n  operationId: getEligibilityDetailsUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/EstimateCalculation\n  method: post\n  operationId: estimateCalculation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/InsuranceDiscovery\n  method: post\n  operationId: insuranceDiscovery\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/GetInusuranceDiscoverySummaryResponse/{requestId}\n\
  \  method: get\n  operationId: getInsuranceDiscoverySummaryResponse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /API/GetInsuranceDiscoveryDetailsURL/{requestId}\n  method: get\n  operationId: getInsuranceDiscoveryDetailsUrl\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /PDFReport/InsuranceDiscovery/{id}\n  method: get\n  operationId: getInsuranceDiscoveryReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /API/MBIInquiry\n  method: post\n  operationId: mbiInquiry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /API/GetMBIResponse/{requestId}\n  method: get\n  operationId: getMBIResponse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/PatientFinderInquiry\n  method: post\n  operationId: patientFinderInquiry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /API/PatientFinderInquiryResults\n  method: post\n  operationId: patientFinderInquiryResults\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n    \
  \  - abnormal\n      - high-value\n    audit: required\n- path: /API/GetPatientFinderResponse/{requestId}\n  method: get\n  operationId: getPatientFinderResponse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /API/GetAllPayers\n  method: get\n  operationId: getAllPayers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/GetPayerStatus\n  method: get\n  operationId: getPayerStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /API/GetPayerStatusStatistics\n  method: get\n  operationId: getPayerStatusStatistics\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /API/SameOrSimilarInquiry\n\
  \  method: post\n  operationId: sameOrSimilarInquiry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /API/GetSameOrSimilarResponse/{requestId}\n  method: get\n  operationId: getSameOrSimilarResponse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /PDFReport/SameorSimilar/{id}\n  method: get\n  operationId: getSameOrSimilarReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /API/GetSameAndSimilarDetailsURL/{requestId}\n  method: get\n  operationId: getSameOrSimilarDetailsUrl\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /API/SNFInquiry\n  method: post\n  operationId: snfInquiry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /API/GetSNFResponse/{requestId}\n  method: get\n  operationId: getSNFResponse\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/pverify/refs/heads/main/agentic-access/pverify-agentic-access.yml
summary_line: 39 operations · 18 acting
tags:
- Healthcare
- Insurance
- Eligibility
- Claims
- EDI
- 270/271
- 276/277
- Revenue Cycle
- Medicare
- Payers
- Insurance Discovery
- Patient Estimation
- HIPAA
- Dental
---
