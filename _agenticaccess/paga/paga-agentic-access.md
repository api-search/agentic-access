---
acting_count: 15
action_class_counts:
  acting: 15
  connected: 8
api_specs:
- filename: paga-openapi.yml
  format: yaml
  label: Paga Collect API
  slug: paga-collect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paga/refs/heads/main/openapi/paga-openapi.yml
- filename: paga-openapi.yml
  format: yaml
  label: Paga Business API
  slug: paga-business-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paga/refs/heads/main/openapi/paga-openapi.yml
- filename: paga-openapi.yml
  format: yaml
  label: Paga Direct Debit API
  slug: paga-direct-debit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/paga/refs/heads/main/openapi/paga-openapi.yml
consequence_counts:
  read: 8
  write: 15
description: Recommended x-agentic-access execution contracts, classified heuristically from the modeled OpenAPI. A governance starting point for exposing Paga's payment APIs to AI agents - review and bind audience per deployment. Money-movement operations default to human-in-the-loop because they debit or disburse real NGN funds. See research/curity/agentic-access/.
human_in_the_loop: 8
kind: agentic-access
layout: agentic-access
method: generated
name: Paga Agentic Access
name_suffix: Agentic Access
notable_actions: []
operation_count: 23
overview: 'Paga exposes 23 API operations that an AI agent could call, of which 15 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 8 read and 15 write.


  8 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Paga
provider_slug: paga
slug: paga-agentic-access
source_filename: paga-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-17'\nmethod: generated\nsource: openapi/paga-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the modeled OpenAPI. A governance starting point for exposing Paga's payment APIs to AI\n  agents - review and bind audience per deployment. Money-movement operations default to\n  human-in-the-loop because they debit or disburse real NGN funds. See research/curity/agentic-access/.\nsummary:\n  operations: 23\n  by_action_class:\n    acting: 15\n    connected: 8\n  by_consequence:\n    write: 15\n    read: 8\n  human_in_the_loop_required: 8\noperations:\n- path: /paymentRequest\n  method: post\n  operationId: requestPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n      - high-value\n    audit: required\n- path:\
  \ /status\n  method: post\n  operationId: checkStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /refund/v2\n  method: post\n  operationId: refundPaymentV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n      - refund\n    audit: required\n- path: /history\n  method: post\n  operationId: retrieveHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /banks\n  method: post\n  operationId: getCollectBanks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /registerPersistentPaymentAccount\n\
  \  method: post\n  operationId: registerPersistentPaymentAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - pii\n    audit: required\n- path: /getPersistentPaymentAccount\n  method: post\n  operationId: getPersistentPaymentAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /updatePersistentPaymentAccount\n  method: post\n  operationId: updatePersistentPaymentAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n    audit: required\n- path: /deletePersistentPaymentAccount\n  method: post\n \
  \ operationId: deletePersistentPaymentAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - destructive\n      - irreversible\n    audit: required\n- path: /chargeDebitMandate\n  method: post\n  operationId: chargeDebitMandate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n      - high-value\n    audit: required\n- path: /getChargeMandateStatus\n  method: post\n  operationId: getChargeMandateStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /disableMandate\n  method: post\n  operationId: disableMandate\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - destructive\n    audit: required\n- path: /paga-webservices/business-rest/secured/moneyTransfer\n  method: post\n  operationId: moneyTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n      - high-value\n    audit: required\n- path: /paga-webservices/business-rest/secured/airtimePurchase\n  method: post\n  operationId: airtimePurchase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - money-movement\n    audit: required\n\
  - path: /paga-webservices/business-rest/secured/merchantPayment\n  method: post\n  operationId: merchantPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n      - high-value\n    audit: required\n- path: /paga-webservices/business-rest/secured/depositToBank\n  method: post\n  operationId: depositToBank\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: required\n      triggers:\n      - money-movement\n      - high-value\n    audit: required\n- path: /paga-webservices/business-rest/secured/validateDepositToBank\n  method: post\n  operationId: validateDepositToBank\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    token:\n      max-ttl: 3600\n    audit: none\n- path: /paga-webservices/business-rest/secured/accountBalance\n  method: post\n  operationId: accountBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paga-webservices/business-rest/secured/getBanks\n  method: post\n  operationId: getBusinessBanks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paga-webservices/business-rest/secured/getMobileOperators\n  method: post\n  operationId: getMobileOperators\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paga-webservices/business-rest/secured/getOperationStatus\n  method: post\n  operationId: getOperationStatus\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paga-webservices/business-rest/secured/transactionHistory\n  method: post\n  operationId: transactionHistory\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /paga-webservices/business-rest/secured/registerCustomer\n  method: post\n  operationId: registerCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - pii\n      - kyc\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/paga/refs/heads/main/agentic-access/paga-agentic-access.yml
summary_line: 23 operations · 15 acting · 8 human-in-the-loop
tags:
- Payments
- Mobile Money
- Fintech
- Collections
- Nigeria
---
