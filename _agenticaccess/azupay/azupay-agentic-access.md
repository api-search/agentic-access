---
acting_count: 25
action_class_counts:
  acting: 25
  connected: 12
api_specs:
- filename: azupay-payment-request.yml
  format: yaml
  label: Azupay PaymentRequest API (AzupayId)
  slug: azupay-payment-request-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azupay/refs/heads/main/openapi/azupay-payment-request.yml
- filename: azupay-payment.yml
  format: yaml
  label: Azupay Payment API (AzupayOut)
  slug: azupay-payment-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azupay/refs/heads/main/openapi/azupay-payment.yml
- filename: azupay-payment-agreement.yml
  format: yaml
  label: Azupay PaymentAgreement & Initiation API (AzupayTo / PayTo)
  slug: azupay-payment-agreement-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azupay/refs/heads/main/openapi/azupay-payment-agreement.yml
- filename: azupay-check-accounts.yml
  format: yaml
  label: Azupay Account Check API (Confirmation of Payee)
  slug: azupay-check-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azupay/refs/heads/main/openapi/azupay-check-accounts.yml
- filename: azupay-reports.yml
  format: yaml
  label: Azupay Report & Balance API
  slug: azupay-reports-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azupay/refs/heads/main/openapi/azupay-reports.yml
- filename: azupay-configuration.yml
  format: yaml
  label: Azupay Clients & API Key Management API
  slug: azupay-configuration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/azupay/refs/heads/main/openapi/azupay-configuration.yml
consequence_counts:
  physical: 17
  read: 12
  safety-critical: 1
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Azupay Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /clients/{clientId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /client/{clientId}/apiKeys
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /clients/{clientId}/lowBalanceAlert/emailAddresses
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment/search
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paymentAgreement
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paymentAgreement/amendment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paymentAgreement/changeStatus
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paymentAgreement/search
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paymentAgreement/{paymentAgreementId}/scheduler
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paymentAgreementRequest
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paymentInitiation
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paymentInitiation/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paymentInitiation/search
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paymentRequest
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /paymentRequest
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paymentRequest/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paymentRequest/search
operation_count: 37
overview: 'Azupay exposes 37 API operations that an AI agent could call, of which 25 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 12 read, 7 write, 17 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Azupay
provider_slug: azupay
slug: azupay-agentic-access
source_filename: azupay-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-24'\nmethod: generated\nsource: openapi/azupay-check-accounts.yml, openapi/azupay-configuration.yml, openapi/azupay-payment-agreement.yml,\n  openapi/azupay-payment-request.yml, openapi/azupay-payment.yml, openapi/azupay-reports.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 37\n  by_action_class:\n    acting: 25\n    connected: 12\n  by_consequence:\n    write: 7\n    physical: 17\n    read: 12\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /accountCheck\n  method: post\n  operationId: checkAccountDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accountEnquiry\n  method: post\n  operationId: enquireAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payIDEnquiry\n  method: post\n  operationId: checkPayID\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client/{clientId}/apiKeys\n  method: post\n  operationId: apiKeysProvision\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n  \
  \    max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client/{clientId}/apiKeys\n  method: get\n  operationId: getApiKeys\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/{clientId}/apiKeys/{apiKeyId}\n  method: get\n  operationId: getApiKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /client/{clientId}/apiKeys/{apiKeyId}\n  method: patch\n  operationId: updateApiKeys\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /client/{clientId}/oauth2\n  method: post\n  operationId: enableClientOAuth2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client/{clientId}/oauth2\n  method: get\n  operationId: getClientOAuth2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clients\n  method: post\n  operationId: createClient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clients/{clientId}\n  method: delete\n\
  \  operationId: deleteClient\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /clients/{clientId}/lowBalanceAlert/emailAddresses\n  method: get\n  operationId: getClientLowBalanceAlertEmailAddresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clients/{clientId}/lowBalanceAlert/emailAddresses\n  method: put\n  operationId: updateClientLowBalanceAlertEmailAddresses\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /clients/{clientId}/lowBalanceAlert/threshold\n  method: get\n  operationId: getClientLowBalanceAlertThreshold\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /clients/{clientId}/lowBalanceAlert/threshold\n  method: put\n  operationId: updateClientLowBalanceAlertThreshold\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paymentAgreement\n  method: post\n  operationId: createPaymentAgreement\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n   \
  \   purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paymentAgreement/amendment\n  method: post\n  operationId: createPaymentAgreementAmendment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paymentAgreement/changeStatus\n  method: post\n  operationId: changeStatusOfPaymentAgreement\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /paymentAgreement/search\n  method: post\n  operationId: searchPaymentAgreement\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paymentAgreement/{paymentAgreementId}/scheduler\n  method: post\n  operationId: createOrUpdatePaymentScheduler\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paymentAgreement/{paymentAgreementId}/scheduler\n  method: get\n  operationId: getPaymentScheduler\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paymentAgreementRequest\n  method: post\n  operationId: createPaymentAgreementRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paymentInitiation\n  method: get\n  operationId: getPaymentInitiation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paymentInitiation\n  method: post\n  operationId: makePaymentInitiation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paymentInitiation/refund\n  method: post\n  operationId: refundPaymentInitation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paymentInitiation/search\n  method: post\n  operationId: searchPaymentInitiation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /paymentRequest\n  method: post\n  operationId: createPayIdPaymentRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paymentRequest\n  method: delete\n  operationId: deletePaymentRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paymentRequest\n  method: get\n  operationId: getPaymentRequest\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paymentRequest/refund\n  method: post\n  operationId: refundPaymentRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paymentRequest/search\n  method: post\n  operationId: searchPaymentRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment\n  method: get\n  operationId: getPayment\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment\n  method: post\n  operationId: makePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment/search\n  method: post\n  operationId: searchPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /balance\n  method: get\n  operationId: getBalance\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /report\n  method: get\n  operationId: getReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /report/download\n  method: get\n  operationId: downloadReport\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/azupay/refs/heads/main/agentic-access/azupay-agentic-access.yml
summary_line: 37 operations · 25 acting · 1 human-in-the-loop
tags:
- Payments
- Australia
- Real-Time Payments
- Account-to-Account
- New Payments Platform
- PayID
- PayTo
- Money Transfer
- Confirmation of Payee
- Open Banking
---
