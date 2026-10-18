---
acting_count: 24
action_class_counts:
  acting: 24
  connected: 33
api_specs:
- filename: memo-bank-account-assessments-api-openapi.yml
  format: yaml
  label: Memo Bank Account assessments API
  slug: memo-bank-account-assessments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memo-bank/refs/heads/main/openapi/memo-bank-account-assessments-api-openapi.yml
- filename: memo-bank-accounts-api-openapi.yml
  format: yaml
  label: Memo Bank Accounts API
  slug: memo-bank-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memo-bank/refs/heads/main/openapi/memo-bank-accounts-api-openapi.yml
- filename: memo-bank-ais-api-openapi.yml
  format: yaml
  label: Memo Bank AIS API
  slug: memo-bank-ais-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memo-bank/refs/heads/main/openapi/memo-bank-ais-api-openapi.yml
- filename: memo-bank-attachments-api-openapi.yml
  format: yaml
  label: Memo Bank Attachments API
  slug: memo-bank-attachments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memo-bank/refs/heads/main/openapi/memo-bank-attachments-api-openapi.yml
- filename: memo-bank-collections-api-openapi.yml
  format: yaml
  label: Memo Bank Collections API
  slug: memo-bank-collections-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memo-bank/refs/heads/main/openapi/memo-bank-collections-api-openapi.yml
- filename: memo-bank-mandate-signature-requests-api-openapi.yml
  format: yaml
  label: Memo Bank Mandate signature requests API
  slug: memo-bank-mandate-signature-requests-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memo-bank/refs/heads/main/openapi/memo-bank-mandate-signature-requests-api-openapi.yml
- filename: memo-bank-pis-api-openapi.yml
  format: yaml
  label: Memo Bank PIS API
  slug: memo-bank-pis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memo-bank/refs/heads/main/openapi/memo-bank-pis-api-openapi.yml
- filename: memo-bank-sandbox-api-openapi.yml
  format: yaml
  label: Memo Bank Sandbox API
  slug: memo-bank-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memo-bank/refs/heads/main/openapi/memo-bank-sandbox-api-openapi.yml
- filename: memo-bank-transactions-api-openapi.yml
  format: yaml
  label: Memo Bank Transactions API
  slug: memo-bank-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memo-bank/refs/heads/main/openapi/memo-bank-transactions-api-openapi.yml
- filename: memo-bank-transfers-api-openapi.yml
  format: yaml
  label: Memo Bank Transfers API
  slug: memo-bank-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memo-bank/refs/heads/main/openapi/memo-bank-transfers-api-openapi.yml
- filename: memo-bank-webhook-api-openapi.yml
  format: yaml
  label: Memo Bank Webhook API
  slug: memo-bank-webhook-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memo-bank/refs/heads/main/openapi/memo-bank-webhook-api-openapi.yml
- filename: memo-bank-webhooks-api-openapi.yml
  format: yaml
  label: Memo Bank Webhooks API
  slug: memo-bank-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memo-bank/refs/heads/main/openapi/memo-bank-webhooks-api-openapi.yml
- filename: memo-bank-wire-transfers-api-openapi.yml
  format: yaml
  label: Memo Bank Wire Transfers API
  slug: memo-bank-wire-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memo-bank/refs/heads/main/openapi/memo-bank-wire-transfers-api-openapi.yml
- filename: memo-bank-ibans-api-openapi.yml
  format: yaml
  label: Memo Bank IBA Ns API
  slug: memo-bank-ibans-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memo-bank/refs/heads/main/openapi/memo-bank-ibans-api-openapi.yml
- filename: memo-bank-oauth2-api-openapi.yml
  format: yaml
  label: Memo Bank O Auth2 API
  slug: memo-bank-oauth2-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/memo-bank/refs/heads/main/openapi/memo-bank-oauth2-api-openapi.yml
consequence_counts:
  physical: 8
  read: 33
  write: 16
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Memo Bank Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/{payment-service}/{payment-product}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v1/{payment-service}/{payment-product}/{paymentId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/sandbox/incoming_transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/transfers/bulks
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /v2/transfers/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/wire_transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/wire_transfers/{id}/attachments
operation_count: 57
overview: 'Memo Bank exposes 57 API operations that an AI agent could call, of which 24 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 33 read, 16 write, and 8 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Memo Bank
provider_slug: memo-bank
slug: memo-bank-agentic-access
source_filename: memo-bank-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: generated\nsource: openapi/memo-bank-account-assessments-api-openapi.yml, openapi/memo-bank-accounts-api-openapi.yml,\n  openapi/memo-bank-ais-api-openapi.yml, openapi/memo-bank-attachments-api-openapi.yml, openapi/memo-bank-collections-api-openapi.yml,\n  openapi/memo-bank-ibans-api-openapi.yml, openapi/memo-bank-mandate-signature-requests-api-openapi.yml,\n  openapi/memo-bank-oauth2-api-openapi.yml, openapi/memo-bank-pis-api-openapi.yml, openapi/memo-bank-sandbox-api-openapi.yml,\n  openapi/memo-bank-transactions-api-openapi.yml, openapi/memo-bank-transfers-api-openapi.yml,\n  openapi/memo-bank-webhooks-api-openapi.yml, openapi/memo-bank-wire-transfers-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations:\
  \ 57\n  by_action_class:\n    acting: 24\n    connected: 33\n  by_consequence:\n    write: 16\n    read: 33\n    physical: 8\n  human_in_the_loop_required: 0\noperations:\n- path: /v2/account_assessments\n  method: post\n  operationId: createAccountAssessment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/account_assessments/{id}\n  method: get\n  operationId: getAccountAssessment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts/{id}\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/accounts\n\
  \  method: get\n  operationId: listAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{accountId}/balances\n  method: get\n  operationId: readAccountBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - AIS\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{accountId}\n  method: get\n  operationId: readAccountDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - AIS\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts/{accountId}/transactions/{transactionId}\n  method: get\n  operationId: readAccountTransactionDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - AIS\n    token:\n      max-ttl: 3600\n    audit: none\n\
  - path: /v1/accounts/{accountId}/transactions\n  method: get\n  operationId: readAccountTransactionsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - AIS\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/accounts\n  method: get\n  operationId: readAccountsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - AIS\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/card-accounts/{accountId}/balances\n  method: get\n  operationId: readCardAccountBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - AIS\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/card-accounts/{accountId}\n  method: get\n  operationId: readCardAccountDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - AIS\n  \
  \  token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/card-accounts/{accountId}/transactions\n  method: get\n  operationId: readCardAccountTransactionsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - AIS\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/card-accounts\n  method: get\n  operationId: readCardAccountsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - AIS\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/attachments\n  method: get\n  operationId: listAttachments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/attachments\n  method: post\n  operationId: createAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/attachments/{id}\n  method: get\n  operationId: getAttachment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/attachments/{id}\n  method: delete\n  operationId: deleteAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/collections/{id}\n  method: get\n  operationId: getCollection\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/collections/{id}\n  method: delete\n\
  \  operationId: cancelCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/collections\n  method: post\n  operationId: createCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/collections/bulks\n  method: post\n  operationId: createCollectionsBulk\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v2/collections/bulks/{id}\n  method: get\n  operationId: getCollectionsBulk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/collections/bulks/{id}/collections\n  method: get\n  operationId: getCollectionsBulkItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/ibans\n  method: get\n  operationId: listIbans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/ibans\n  method: post\n  operationId: createIban\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v2/ibans/{id}\n  method: get\n  operationId: getIban\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/ibans/{id}\n  method: delete\n  operationId: deleteIban\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/ibans/{id}\n  method: patch\n  operationId: updateIban\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/mandate_signature_requests\n  method: get\n  operationId:\
  \ listMandateSignatureRequests\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/mandate_signature_requests\n  method: post\n  operationId: createMandateSignatureRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/mandate_signature_requests/{id}\n  method: get\n  operationId: getMandateSignatureRequest\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/mandate_signature_requests/{id}\n  method: delete\n  operationId: deleteMandateSignatureRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/mandate_signature_requests/{id}/renewals\n  method: post\n  operationId: renewMandateSignatureRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /oauth2/token\n  method: post\n  operationId: createToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/{payment-service}/{payment-product}/{paymentId}\n  method: get\n  operationId:\
  \ getPaymentInformation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/{payment-service}/{payment-product}/{paymentId}\n  method: delete\n  operationId: cancelPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - PIS\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/{payment-service}/{payment-product}/{paymentId}/status\n  method: get\n  operationId: getPaymentInitiationStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/{payment-service}/{payment-product}\n  method: post\n  operationId: initiatePayment\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/sandbox/incoming_collections\n  method: post\n  operationId: createIncomingCollection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/sandbox/incoming_transfers\n  method: post\n  operationId: createIncomingTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/transactions/{id}\n  method: get\n  operationId: getTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/transactions\n  method: get\n  operationId: listTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/transfers/{id}\n  method: get\n  operationId: getTransfer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/transfers/{id}\n  method: delete\n  operationId: cancelTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n \
  \     max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/transfers\n  method: post\n  operationId: createTransferV2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/transfers/bulks\n  method: post\n  operationId: createTransfersBulk\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v2/transfers/{id}/proof\n  method: get\n  operationId: getProofOfTransfer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/transfers/bulks/{id}\n  method: get\n  operationId: getTransfersBulk\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/transfers/bulks/{id}/transfers\n  method: get\n  operationId: getTransfersBulkItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/webhooks\n  method: post\n  operationId: createWebhook\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/webhooks/{id}\n  method: get\n  operationId: getWebhook\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/webhooks/{id}\n  method: delete\n  operationId: deleteWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/wire_transfers\n  method: post\n  operationId: createWireTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/wire_transfers/{id}/attachments\n  method: post\n  operationId: createWireTransferAttachment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/wire_transfers/{id}/proof\n  method: get\n  operationId: getProofOfWireTransfer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/wire_transfers/{id}\n  method: get\n  operationId: getWireTransfer\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/memo-bank/refs/heads/main/agentic-access/memo-bank-agentic-access.yml
summary_line: 57 operations · 24 acting
tags:
- Company
- Fintech Insurtech
- Banking
- Business Banking
- Payments
- SEPA
- SEPA Direct Debit
- virtual-iban
- Wire Transfers
- Open Banking
- PSD2
- Berlin Group
- Webhook
- MCP
- France
---
