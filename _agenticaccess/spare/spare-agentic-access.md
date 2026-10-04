---
acting_count: 18
action_class_counts:
  acting: 18
  connected: 45
api_specs:
- filename: spare-account-api-openapi.yml
  format: yaml
  label: Spare Account API
  slug: spare-account-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-account-api-openapi.yml
- filename: spare-accountinformationreport-api-openapi.yml
  format: yaml
  label: Spare AccountInformationReport API
  slug: spare-accountinformationreport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-accountinformationreport-api-openapi.yml
- filename: spare-balance-api-openapi.yml
  format: yaml
  label: Spare Balance API
  slug: spare-balance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-balance-api-openapi.yml
- filename: spare-beneficiary-api-openapi.yml
  format: yaml
  label: Spare Beneficiary API
  slug: spare-beneficiary-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-beneficiary-api-openapi.yml
- filename: spare-cert-api-openapi.yml
  format: yaml
  label: Spare Cert API
  slug: spare-cert-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-cert-api-openapi.yml
- filename: spare-connection-api-openapi.yml
  format: yaml
  label: Spare Connection API
  slug: spare-connection-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-connection-api-openapi.yml
- filename: spare-consent-api-openapi.yml
  format: yaml
  label: Spare Consent API
  slug: spare-consent-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-consent-api-openapi.yml
- filename: spare-customer-api-openapi.yml
  format: yaml
  label: Spare Customer API
  slug: spare-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-customer-api-openapi.yml
- filename: spare-parties-api-openapi.yml
  format: yaml
  label: Spare Parties API
  slug: spare-parties-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-parties-api-openapi.yml
- filename: spare-payment-api-openapi.yml
  format: yaml
  label: Spare Payment API
  slug: spare-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-payment-api-openapi.yml
- filename: spare-provider-api-openapi.yml
  format: yaml
  label: Spare Provider API
  slug: spare-provider-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-provider-api-openapi.yml
- filename: spare-request-api-openapi.yml
  format: yaml
  label: Spare Request API
  slug: spare-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-request-api-openapi.yml
- filename: spare-riskreport-api-openapi.yml
  format: yaml
  label: Spare RiskReport API
  slug: spare-riskreport-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-riskreport-api-openapi.yml
- filename: spare-statement-api-openapi.yml
  format: yaml
  label: Spare Statement API
  slug: spare-statement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-statement-api-openapi.yml
- filename: spare-token-api-openapi.yml
  format: yaml
  label: Spare Token API
  slug: spare-token-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-token-api-openapi.yml
- filename: spare-transaction-api-openapi.yml
  format: yaml
  label: Spare Transaction API
  slug: spare-transaction-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-transaction-api-openapi.yml
- filename: spare-direct-debit-api-openapi.yml
  format: yaml
  label: Spare Direct Debit API
  slug: spare-direct-debit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/openapi/spare-direct-debit-api-openapi.yml
consequence_counts:
  physical: 2
  read: 45
  safety-critical: 1
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Spare Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /api/v1.0/ais/Consent/Revoke
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1.0/pis/Consent/Create
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /api/v1.0/pis/Request/Create
operation_count: 63
overview: 'Spare exposes 63 API operations that an AI agent could call, of which 18 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 45 read, 15 write, 2 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Spare
provider_slug: spare
slug: spare-agentic-access
source_filename: spare-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/spare-account-api-openapi.yml, openapi/spare-accountinformationreport-api-openapi.yml,\n  openapi/spare-balance-api-openapi.yml, openapi/spare-beneficiary-api-openapi.yml, openapi/spare-cert-api-openapi.yml,\n  openapi/spare-connection-api-openapi.yml, openapi/spare-consent-api-openapi.yml, openapi/spare-customer-api-openapi.yml,\n  openapi/spare-direct-debit-api-openapi.yml, openapi/spare-parties-api-openapi.yml, openapi/spare-payment-api-openapi.yml,\n  openapi/spare-provider-api-openapi.yml, openapi/spare-request-api-openapi.yml, openapi/spare-riskreport-api-openapi.yml,\n  openapi/spare-statement-api-openapi.yml, openapi/spare-token-api-openapi.yml, openapi/spare-transaction-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\n\
  summary:\n  operations: 63\n  by_action_class:\n    connected: 45\n    acting: 18\n  by_consequence:\n    read: 45\n    write: 15\n    safety-critical: 1\n    physical: 2\n  human_in_the_loop_required: 1\noperations:\n- path: /api/v1.0/ais/Account/Get\n  method: get\n  operationId: getApiV10AisAccountGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/ais/Account/List\n  method: get\n  operationId: getApiV10AisAccountList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2.0/ais/Account/Get\n  method: get\n  operationId: getApiV20AisAccountGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2.0/ais/Account/List\n  method: get\n  operationId: getApiV20AisAccountList\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/ais/AccountInformationReport/Create\n  method: post\n  operationId: postApiV10AisAccountInformationReportCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/ais/AccountInformationReport/Get\n  method: get\n  operationId: getApiV10AisAccountInformationReportGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/ais/AccountInformationReport/File\n  method: get\n  operationId: getApiV10AisAccountInformationReportFile\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/ais/AccountInformationReport/List\n  method: post\n  operationId: postApiV10AisAccountInformationReportList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/ais/AccountInformationReport/Status\n  method: get\n  operationId: getApiV10AisAccountInformationReportStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/ais/Balance/Get\n  method: get\n  operationId: getApiV10AisBalanceGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/ais/Balance/History\n  method: get\n  operationId: getApiV10AisBalanceHistory\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2.0/ais/Balance/Get\n  method: get\n  operationId: getApiV20AisBalanceGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/ais/Beneficiary/Get\n  method: get\n  operationId: getApiV10AisBeneficiaryGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/authentication/Jwks\n  method: get\n  operationId: getApiV10AuthenticationJwks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/ais/Connection/Create\n  method: post\n  operationId: postApiV10AisConnectionCreate\n  x-agentic-access:\n    action-class: acting\n  \
  \  consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/ais/Connection/Get\n  method: get\n  operationId: getApiV10AisConnectionGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/ais/Connection/List\n  method: get\n  operationId: getApiV10AisConnectionList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/ais/Connection/Delete\n  method: delete\n  operationId: deleteApiV10AisConnectionDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/ais/Consent/Create\n  method: post\n  operationId: postApiV10AisConsentCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/ais/Consent/List\n  method: get\n  operationId: getApiV10AisConsentList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/ais/Consent/Get\n  method: get\n  operationId: getApiV10AisConsentGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/ais/Consent/Revoke\n  method: patch\n  operationId:\
  \ patchApiV10AisConsentRevoke\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /api/v1.0/pis/Consent/Create\n  method: post\n  operationId: postApiV10PisConsentCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/pis/Consent/List\n  method: get\n  operationId: getApiV10PisConsentList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /api/v1.0/pis/Consent/Get\n  method: get\n  operationId: getApiV10PisConsentGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/ais/Consent/CreateShortLivedConsent\n  method: post\n  operationId: postApiV10AisConsentCreateShortLivedConsent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/ais/Consent/CreateLongLivedConsent\n  method: post\n  operationId: postApiV10AisConsentCreateLongLivedConsent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n \
  \     - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/ais/Customer/Create\n  method: post\n  operationId: postApiV10AisCustomerCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/ais/Customer/List\n  method: get\n  operationId: getApiV10AisCustomerList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/ais/Customer/Get\n  method: get\n  operationId: getApiV10AisCustomerGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/ais/Customer/Update\n  method: patch\n  operationId: patchApiV10AisCustomerUpdate\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/ais/Customer/Delete\n  method: delete\n  operationId: deleteApiV10AisCustomerDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/ais/DirectDebit/Get\n  method: get\n  operationId: getApiV10AisDirectDebitGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/ais/Parties/Get\n  method: get\n  operationId: getApiV10AisPartiesGet\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/pis/Payment/List\n  method: post\n  operationId: postApiV10PisPaymentList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/pis/Payment/Get\n  method: get\n  operationId: getApiV10PisPaymentGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/ais/Provider/List\n  method: get\n  operationId: getApiV10AisProviderList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/pis/Provider/List\n  method: get\n  operationId: getApiV10PisProviderList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/ais/Request/Create\n  method: post\n  operationId: postApiV10AisRequestCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/ais/Request/List\n  method: get\n  operationId: getApiV10AisRequestList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/ais/Request/Get\n  method: get\n  operationId: getApiV10AisRequestGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/ais/Request/Update\n  method: put\n  operationId: putApiV10AisRequestUpdate\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/ais/Request/Delete\n  method: delete\n  operationId: deleteApiV10AisRequestDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/pis/Request/Create\n  method: post\n  operationId: postApiV10PisRequestCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/pis/Request/List\n  method: get\n  operationId: getApiV10PisRequestList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/pis/Request/Get\n  method: get\n  operationId: getApiV10PisRequestGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/pis/Request/Delete\n  method: get\n  operationId: getApiV10PisRequestDelete\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/ais/Request/CreateShortLivedRequest\n  method: post\n  operationId: postApiV10AisRequestCreateShortLivedRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/ais/Request/CreateLongLivedRequest\n  method: post\n  operationId: postApiV10AisRequestCreateLongLivedRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/ais/RiskReport/Create\n  method: get\n  operationId: getApiV10AisRiskReportCreate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/ais/RiskReport/Get\n  method: get\n  operationId: getApiV10AisRiskReportGet\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/ais/RiskReport/Export\n  method: get\n  operationId: getApiV10AisRiskReportExport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/ais/RiskReport/List\n  method: post\n  operationId: postApiV10AisRiskReportList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/ais/RiskReport/Status\n  method: get\n  operationId: getApiV10AisRiskReportStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/ais/RiskReport/Delete\n  method: delete\n  operationId: deleteApiV10AisRiskReportDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /api/v1.0/ais/Statement/File\n  method: get\n  operationId: getApiV10AisStatementFile\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/authentication/Token\n  method: get\n  operationId: getApiV10AuthenticationToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/authentication/Refresh\n  method: get\n  operationId: getApiV10AuthenticationRefresh\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/ais/Transaction/Get\n  method: get\n  operationId:\
  \ getApiV10AisTransactionGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/ais/Transaction/List\n  method: post\n  operationId: postApiV10AisTransactionList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v1.0/ais/Transaction/Salaries\n  method: get\n  operationId: getApiV10AisTransactionSalaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2.0/ais/Transaction/Get\n  method: get\n  operationId: getApiV20AisTransactionGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /api/v2.0/ais/Transaction/List\n  method: post\n  operationId: postApiV20AisTransactionList\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/spare/refs/heads/main/agentic-access/spare-agentic-access.yml
summary_line: 63 operations · 18 acting · 1 human-in-the-loop
tags:
- Open Banking
- Open Finance
- Account Information
- Payment Initiation
- AISP
- PISP
- Consent
- Bank Data
- Transaction
- Balances
- Payments
- Fintech
- MENA
- Saudi Arabia
- Bahrain
- United Arab Emirates
---
