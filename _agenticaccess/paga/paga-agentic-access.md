---
acting_count: 17
action_class_counts:
  acting: 17
  connected: 6
api_specs:
- filename: paga-business-api-openapi.yml
  format: yaml
  label: Paga Business API
  slug: paga-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paga/refs/heads/main/openapi/paga-business-api-openapi.yml
- filename: paga-collect-api-openapi.yml
  format: yaml
  label: Paga Collect API
  slug: paga-collect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paga/refs/heads/main/openapi/paga-collect-api-openapi.yml
- filename: paga-direct-debit-api-openapi.yml
  format: yaml
  label: Paga Direct Debit API
  slug: paga-direct-debit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paga/refs/heads/main/openapi/paga-direct-debit-api-openapi.yml
- filename: paga-reference-api-openapi.yml
  format: yaml
  label: Paga Reference API
  slug: paga-reference-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paga/refs/heads/main/openapi/paga-reference-api-openapi.yml
consequence_counts:
  physical: 13
  read: 6
  safety-critical: 1
  write: 3
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Paga Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /disableMandate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /chargeDebitMandate
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /deletePersistentPaymentAccount
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /getChargeMandateStatus
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paga-webservices/business-rest/secured/airtimePurchase
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paga-webservices/business-rest/secured/depositToBank
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paga-webservices/business-rest/secured/merchantPayment
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paga-webservices/business-rest/secured/moneyTransfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paga-webservices/business-rest/secured/validateDepositToBank
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /paymentRequest
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /refund/v2
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /registerPersistentPaymentAccount
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /status
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /updatePersistentPaymentAccount
operation_count: 23
overview: 'Paga exposes 23 API operations that an AI agent could call, of which 17 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 6 read, 3 write, 13 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Paga
provider_slug: paga
slug: paga-agentic-access
source_filename: paga-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-09-23'\nmethod: generated\nsource: openapi/paga-business-api-openapi.yml, openapi/paga-collect-api-openapi.yml, openapi/paga-direct-debit-api-openapi.yml,\n  openapi/paga-reference-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 23\n  by_action_class:\n    acting: 17\n    connected: 6\n  by_consequence:\n    physical: 13\n    write: 3\n    read: 6\n    safety-critical: 1\n  human_in_the_loop_required: 1\noperations:\n- path: /paga-webservices/business-rest/secured/moneyTransfer\n  method: post\n  operationId: moneyTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paga-webservices/business-rest/secured/airtimePurchase\n  method: post\n  operationId: airtimePurchase\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paga-webservices/business-rest/secured/merchantPayment\n  method: post\n  operationId: merchantPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /paga-webservices/business-rest/secured/depositToBank\n  method: post\n  operationId: depositToBank\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paga-webservices/business-rest/secured/validateDepositToBank\n  method: post\n  operationId: validateDepositToBank\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paga-webservices/business-rest/secured/accountBalance\n  method: post\n\
  \  operationId: accountBalance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paga-webservices/business-rest/secured/transactionHistory\n  method: post\n  operationId: transactionHistory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paga-webservices/business-rest/secured/registerCustomer\n  method: post\n  operationId: registerCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /paymentRequest\n  method: post\n  operationId: requestPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /status\n  method: post\n  operationId: checkStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /refund/v2\n  method: post\n  operationId: refundPaymentV2\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /history\n  method: post\n  operationId: retrieveHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /registerPersistentPaymentAccount\n  method: post\n  operationId: registerPersistentPaymentAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getPersistentPaymentAccount\n  method: post\n  operationId:\
  \ getPersistentPaymentAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /updatePersistentPaymentAccount\n  method: post\n  operationId: updatePersistentPaymentAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /deletePersistentPaymentAccount\n  method: post\n  operationId: deletePersistentPaymentAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /chargeDebitMandate\n  method: post\n  operationId: chargeDebitMandate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /getChargeMandateStatus\n  method: post\n  operationId: getChargeMandateStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /disableMandate\n  method: post\n  operationId: disableMandate\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /banks\n  method: post\n  operationId: getCollectBanks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paga-webservices/business-rest/secured/getBanks\n  method: post\n  operationId: getBusinessBanks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paga-webservices/business-rest/secured/getMobileOperators\n  method: post\n  operationId: getMobileOperators\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paga-webservices/business-rest/secured/getOperationStatus\n\
  \  method: post\n  operationId: getOperationStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paga/refs/heads/main/agentic-access/paga-agentic-access.yml
summary_line: 23 operations · 17 acting · 1 human-in-the-loop
tags:
- Payments
- Mobile Money
- Fintech
- Collection
- Nigeria
---
