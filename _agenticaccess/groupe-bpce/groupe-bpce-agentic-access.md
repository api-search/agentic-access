---
acting_count: 16
action_class_counts:
  acting: 16
  connected: 33
api_specs:
- filename: groupe-bpce-aisp-api-openapi.yml
  format: yaml
  label: Groupe BPCE AISP API
  slug: groupe-bpce-aisp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groupe-bpce/refs/heads/main/openapi/groupe-bpce-aisp-api-openapi.yml
- filename: groupe-bpce-cbpii-api-openapi.yml
  format: yaml
  label: Groupe BPCE CBPII API
  slug: groupe-bpce-cbpii-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groupe-bpce/refs/heads/main/openapi/groupe-bpce-cbpii-api-openapi.yml
- filename: groupe-bpce-external-accounts-api-openapi.yml
  format: yaml
  label: Groupe BPCE External Accounts API
  slug: groupe-bpce-external-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groupe-bpce/refs/heads/main/openapi/groupe-bpce-external-accounts-api-openapi.yml
- filename: groupe-bpce-internal-accounts-api-openapi.yml
  format: yaml
  label: Groupe BPCE Internal Accounts API
  slug: groupe-bpce-internal-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groupe-bpce/refs/heads/main/openapi/groupe-bpce-internal-accounts-api-openapi.yml
- filename: groupe-bpce-pisp-api-openapi.yml
  format: yaml
  label: Groupe BPCE PISP API
  slug: groupe-bpce-pisp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groupe-bpce/refs/heads/main/openapi/groupe-bpce-pisp-api-openapi.yml
- filename: groupe-bpce-registration-api-openapi.yml
  format: yaml
  label: Groupe BPCE Registration API
  slug: groupe-bpce-registration-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groupe-bpce/refs/heads/main/openapi/groupe-bpce-registration-api-openapi.yml
- filename: groupe-bpce-transfers-api-openapi.yml
  format: yaml
  label: Groupe BPCE Transfers API
  slug: groupe-bpce-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/groupe-bpce/refs/heads/main/openapi/groupe-bpce-transfers-api-openapi.yml
consequence_counts:
  physical: 9
  read: 33
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Groupe Bpce Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /funds-confirmations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment-requests
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /payment-requests/{paymentRequestResourceId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payment-requests/{paymentRequestResourceId}/confirmation
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transferRequests
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /transferRequests/{transferRequestId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transferRequests/{transferRequestId}/confirmations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transferRequests/{transferRequestId}/transferRequestLines
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /transferRequests/{transferRequestId}/transferRequestLines/{transferRequestLineId}
operation_count: 49
overview: 'Groupe BPCE exposes 49 API operations that an AI agent could call, of which 16 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 33 read, 7 write, and 9 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Groupe BPCE
provider_slug: groupe-bpce
slug: groupe-bpce-agentic-access
source_filename: groupe-bpce-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-09'\nmethod: generated\nsource: openapi/groupe-bpce-natixis-psd2-accounts-openapi.yml, openapi/groupe-bpce-natixis-wealth-management-psd2-accounts-openapi.yml,\n  openapi/groupe-bpce-open-finance-transfer-openapi.yml, openapi/groupe-bpce-psd2-accounts-openapi.yml,\n  openapi/groupe-bpce-psd2-funds-availability-openapi.yml, openapi/groupe-bpce-psd2-payments-openapi.yml,\n  openapi/groupe-bpce-psd2-registration-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 49\n  by_action_class:\n    connected: 33\n    acting: 16\n  by_consequence:\n    read: 33\n    write: 7\n    physical: 9\n  human_in_the_loop_required: 0\noperations:\n- path: /accounts\n  method: get\n  operationId: accountsGet\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - aisp\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountResourceId}/owners\n  method: get\n  operationId: accountsOwnersGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - aisp\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountResourceId}/balances\n  method: get\n  operationId: accountsBalancesGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - aisp\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountResourceId}/transactions\n  method: get\n  operationId: accountsTransactionsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - aisp\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountResourceId}/transactions/{transactionResourceId}/details\n\
  \  method: get\n  operationId: accountsTransactionsDetailsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - aisp\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountResourceId}/overdrafts\n  method: get\n  operationId: accountsOverdraftsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - aisp\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /consents\n  method: put\n  operationId: consentsPut\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - aisp\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /end-user-identity\n  method: get\n  operationId: EndUserIdentityGet\n  x-agentic-access:\n    action-class: connected\n  \
  \  consequence: read\n    subject: optional\n    scope:\n    - aisp\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trusted-beneficiaries\n  method: get\n  operationId: trustedBeneficiariesGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - aisp\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts\n  method: get\n  operationId: accountsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - aisp\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountResourceId}/owners\n  method: get\n  operationId: accountsOwnersGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - aisp\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountResourceId}/balances\n  method: get\n  operationId: accountsBalancesGet\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - aisp\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountResourceId}/transactions\n  method: get\n  operationId: accountsTransactionsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - aisp\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountResourceId}/transactions/{transactionResourceId}/details\n  method: get\n  operationId: accountsTransactionsDetailsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - aisp\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountResourceId}/overdrafts\n  method: get\n  operationId: accountsOverdraftsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - aisp\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /consents\n  method: put\n  operationId: consentsPut\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - aisp\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /end-user-identity\n  method: get\n  operationId: EndUserIdentityGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - aisp\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trusted-beneficiaries\n  method: get\n  operationId: trustedBeneficiariesGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - aisp\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /internalAccounts\n  method: get\n  operationId: getInternalAccounts\n  x-agentic-access:\n    action-class: connected\n   \
  \ consequence: read\n    subject: optional\n    scope:\n    - moneyTransfer.internalAccounts:READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /externalAccounts\n  method: get\n  operationId: getExternalAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - moneyTransfer.externalAccounts:READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /externalAccounts\n  method: post\n  operationId: createExternalAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - moneyTransfer.externalAccounts:WRITE\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transferRequests\n  method: post\n  operationId: createTransferRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n  \
  \  subject: required\n    scope:\n    - moneyTransfer.transferRequests:WRITE\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transferRequests/{transferRequestId}/errors\n  method: get\n  operationId: getTransferRequestErrors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - moneyTransfer.transferRequests:READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transferRequests/{transferRequestId}\n  method: get\n  operationId: getTransferRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - moneyTransfer.transferRequests:READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transferRequests/{transferRequestId}\n  method: delete\n  operationId:\
  \ deleteTransferRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - moneyTransfer.transferRequests:DELETE\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transferRequests/{transferRequestId}/confirmations\n  method: post\n  operationId: createTransferRequestConfirmation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - moneyTransfer.transferRequests.confirmations:WRITE\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transferRequests/{transferRequestId}/transferRequestLines\n\
  \  method: post\n  operationId: createTransferRequestTransferRequestLine\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - moneyTransfer.transferRequests:WRITE\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transferRequests/{transferRequestId}/transferRequestLines\n  method: get\n  operationId: getTransferRequestTransferRequestLines\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - moneyTransfer.transferRequests:READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transferRequests/{transferRequestId}/transferRequestLines/{transferRequestLineId}\n  method: get\n  operationId: getTransferRequestTransferRequestLine\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    scope:\n    - moneyTransfer.transferRequests:READ\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transferRequests/{transferRequestId}/transferRequestLines/{transferRequestLineId}\n  method: delete\n  operationId: deleteTransferRequestTransferRequestLine\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - moneyTransfer.transferRequests:DELETE\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts\n  method: get\n  operationId: accountsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - aisp\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountResourceId}/owners\n \
  \ method: get\n  operationId: accountsOwnersGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - aisp\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountResourceId}/balances\n  method: get\n  operationId: accountsBalancesGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - aisp\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountResourceId}/transactions\n  method: get\n  operationId: accountsTransactionsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - aisp\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountResourceId}/transactions/{transactionResourceId}/details\n  method: get\n  operationId: accountsTransactionsDetailsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n\
  \    scope:\n    - aisp\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{accountResourceId}/overdrafts\n  method: get\n  operationId: accountsOverdraftsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - aisp\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /consents\n  method: put\n  operationId: consentsPut\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - aisp\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /end-user-identity\n  method: get\n  operationId: EndUserIdentityGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - aisp\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trusted-beneficiaries\n  method:\
  \ get\n  operationId: trustedBeneficiariesGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - aisp\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /funds-confirmations\n  method: post\n  operationId: fundsConfirmationsPost\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - cbpii\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment-requests\n  method: post\n  operationId: paymentRequestsPost\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - pisp\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment-requests/{paymentRequestResourceId}\n  method: get\n  operationId: paymentRequestsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - pisp\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /payment-requests/{paymentRequestResourceId}\n  method: put\n  operationId: paymentRequestPut\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - pisp\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment-requests/{paymentRequestResourceId}/confirmation\n  method: post\n  operationId: paymentRequestConfirmationPost\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: physical\n    subject: required\n    scope:\n    - pisp\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /payment-requests/{paymentRequestResourceId}/transactions\n  method: get\n  operationId: paymentRequestTransactionsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - pisp\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /register\n  method: post\n  operationId: registrationPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /register/{clientId}\n  method: get\n \
  \ operationId: registrationGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /register/{clientId}\n  method: put\n  operationId: registrationPut\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /register/{clientId}\n  method: delete\n  operationId: registrationDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/groupe-bpce/refs/heads/main/agentic-access/groupe-bpce-agentic-access.yml
summary_line: 49 operations · 16 acting
tags:
- Company
- Banking
- Financial Services
- Open Banking
- PSD2
- Payments
- Insurance
- France
---
