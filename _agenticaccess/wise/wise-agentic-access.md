---
acting_count: 147
action_class_counts:
  acting: 147
  connected: 91
api_specs:
- filename: wise-platform-openapi.yml
  format: yaml
  label: Wise Profiles API
  slug: profiles
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wise/refs/heads/main/openapi/wise-platform-openapi.yml
- filename: wise-platform-openapi.yml
  format: yaml
  label: Wise Recipients API
  slug: recipients
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wise/refs/heads/main/openapi/wise-platform-openapi.yml
- filename: wise-platform-openapi.yml
  format: yaml
  label: Wise Quotes API
  slug: quotes
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wise/refs/heads/main/openapi/wise-platform-openapi.yml
- filename: wise-platform-openapi.yml
  format: yaml
  label: Wise Transfers API
  slug: transfers
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wise/refs/heads/main/openapi/wise-platform-openapi.yml
- filename: wise-platform-openapi.yml
  format: yaml
  label: Wise Balances API
  slug: balances
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wise/refs/heads/main/openapi/wise-platform-openapi.yml
- filename: wise-platform-openapi.yml
  format: yaml
  label: Wise Multi-Currency Account API
  slug: multi-currency-account
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wise/refs/heads/main/openapi/wise-platform-openapi.yml
- filename: wise-platform-openapi.yml
  format: yaml
  label: Wise Statements API
  slug: statements
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wise/refs/heads/main/openapi/wise-platform-openapi.yml
- filename: wise-platform-openapi.yml
  format: yaml
  label: Wise Cards API
  slug: cards
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wise/refs/heads/main/openapi/wise-platform-openapi.yml
- filename: wise-platform-openapi.yml
  format: yaml
  label: Wise Webhooks API
  slug: webhooks
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wise/refs/heads/main/openapi/wise-platform-openapi.yml
- filename: wise-platform-openapi.yml
  format: yaml
  label: Wise Simulation API
  slug: simulation
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/wise/refs/heads/main/openapi/wise-platform-openapi.yml
consequence_counts:
  physical: 25
  read: 91
  safety-critical: 6
  write: 116
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 6
kind: agentic-access
layout: agentic-access
method: generated
name: Wise Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /twcard-data/v1/sensitive-card-data/preset-pin
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v3/spend/applications/{clientId}/spend-controls/rules
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v3/spend/applications/{clientId}/spend-controls/rules/apply
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v3/spend/applications/{clientId}/spend-controls/rules/unapply
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v3/spend/applications/{clientId}/spend-controls/rules/{ruleId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v3/spend/profiles/{profileId}/cards/{cardToken}/reset-pin-count
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /twcard-data/v1/push-provisioning/encrypted-payload/apple-pay
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /twcard-data/v1/push-provisioning/encrypted-payload/google-pay
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/borderless-accounts/{borderlessAccountId}/conversions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/profiles/{profileId}/account-details-orders
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/profiles/{profileId}/account-details/payments/{paymentId}/returns
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/profiles/{profileId}/batch-groups/{batchGroupId}/payment-initiations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/profiles/{profileId}/partner-licence-transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/profiles/{profileId}/payin-sessions/{payinSessionId}/paynow
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/settlements
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/simulation/profiles/{profileId}/bank-transactions/import
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/simulation/profiles/{profileId}/swift-in
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/transfer-requirements
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/transfers/{transferId}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/profiles/{profileId}/third-party-transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/profiles/{profileId}/batch-groups/{batchGroupId}/transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/profiles/{profileId}/batch-payments/{batchGroupId}/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/profiles/{profileId}/transfers/{transferId}/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v3/profiles/{profileId}/verification-status/bank-transfer
operation_count: 238
overview: 'Wise exposes 238 API operations that an AI agent could call, of which 147 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 91 read, 116 write, 25 physical, and 6 safety-critical.


  6 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Wise
provider_slug: wise
slug: wise-agentic-access
source_filename: wise-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/wise-platform-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 238\n  by_action_class:\n    acting: 147\n    connected: 91\n  by_consequence:\n    write: 116\n    read: 91\n    physical: 25\n    safety-critical: 6\n  human_in_the_loop_required: 6\noperations:\n- path: /v3/spend/profiles/{profileId}/3dsecure/challenge-result\n  method: post\n  operationId: 3dsChallengeResultPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/profiles/{profileId}/activities\n\
  \  method: get\n  operationId: activityList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/profiles/{profileId}/additional-verification/upload-evidences\n  method: post\n  operationId: verificationUploadEvidencesV3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v5/profiles/{profileId}/additional-verification/upload-evidences\n  method: post\n  operationId: verificationUploadEvidences\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n   \
  \ audit: required\n- path: /v3/profiles/{profileId}/verification-status/upload-document\n  method: post\n  operationId: verificationUploadDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/profiles/{profileId}/verification-status/required-evidences\n  method: get\n  operationId: verificationGetRequiredEvidences\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/addresses\n  method: post\n  operationId: addressCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n    \
  \  - abnormal\n      - high-value\n    audit: required\n- path: /v1/addresses\n  method: get\n  operationId: addressList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/addresses/{addressId}\n  method: get\n  operationId: addressGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/address-requirements\n  method: get\n  operationId: addressRequirementsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/address-requirements\n  method: post\n  operationId: addressRequirementsPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/profiles/{profileId}/balances\n  method: post\n  operationId: balanceCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/profiles/{profileId}/balances\n  method: get\n  operationId: balanceList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/profiles/{profileId}/balances/{balanceId}\n  method: get\n  operationId: balanceGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/profiles/{profileId}/balances/{balanceId}\n  method: delete\n\
  \  operationId: balanceDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/profiles/{profileId}/balance-movements\n  method: post\n  operationId: balanceMovement\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/profiles/{profileId}/balance-capacity\n  method: get\n  operationId: balanceCapacity\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/profiles/{profileId}/excess-money-account\n  method: post\n\
  \  operationId: excessMoneyAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/profiles/{profileId}/total-funds/{currency}\n  method: get\n  operationId: totalFunds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/borderless-accounts\n  method: get\n  operationId: balanceGetV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/borderless-accounts/{borderlessAccountId}/conversions\n  method: post\n  operationId: balanceConvertV1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/profiles/{profileId}/balances/hold-limit-breach\n  method: post\n  operationId: holdLimitBreachList\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/profiles/{profileId}/balances/hold-limit-breach/{holdLimitBreachId}\n  method: post\n  operationId: holdLimitBreachClose\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/profiles/{profileId}/balance-statements/{balanceId}/statement.json\n  method: get\n  operationId: balanceStatementGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/profiles/{profileId}/account-details-orders\n  method: post\n  operationId: bankAccountDetailsOrderCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/profiles/{profileId}/account-details-orders\n  method: get\n  operationId: bankAccountDetailsOrdersListV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n \
  \   audit: none\n- path: /v3/profiles/{profileId}/bank-details\n  method: post\n  operationId: bankAccountDetailsBankDetailsCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/profiles/{profileId}/account-details\n  method: get\n  operationId: bankAccountDetailsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/profiles/{profileId}/account-details-orders\n  method: get\n  operationId: bankAccountDetailsOrdersList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/profiles/{profileId}/account-details/payments/{paymentId}/returns\n\
  \  method: post\n  operationId: bankAccountDetailsReturnsCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/profiles/{profileId}/batch-groups\n  method: post\n  operationId: batchGroupCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/profiles/{profileId}/batch-groups/{batchGroupId}\n  method: get\n  operationId: batchGroupGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /v3/profiles/{profileId}/batch-groups/{batchGroupId}\n  method: patch\n  operationId: batchGroupUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/profiles/{profileId}/batch-groups/{batchGroupId}/transfers\n  method: post\n  operationId: batchGroupTransferCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/profiles/{profileId}/batch-payments/{batchGroupId}/payments\n  method: post\n  operationId: batchGroupFund\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/profiles/{profileId}/batch-groups/{batchGroupId}/payment-initiations\n  method: post\n  operationId: batchGroupPaymentInitiationCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/profiles/{profileId}/batch-groups/{batchGroupId}/payment-initiations/{paymentInitiationId}\n  method: get\n  operationId: batchGroupPaymentInitiationGet\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/settlements\n  method: post\n  operationId: bulkSettlementJournalCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/spend/profiles/{profileId}/cards\n  method: get\n  operationId: cardList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/spend/profiles/{profileId}/cards/{cardToken}\n  method: get\n  operationId: cardGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/spend/profiles/{profileId}/cards/{cardToken}/status\n\
  \  method: put\n  operationId: cardStatusUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/spend/profiles/{profileId}/cards/{cardToken}/reset-pin-count\n  method: post\n  operationId: cardPinCountReset\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v3/spend/profiles/{profileId}/cards/{cardToken}/spending-permissions\n  method: get\n  operationId: cardPermissionsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v3/spend/profiles/{profileId}/cards/{cardToken}/spending-permissions\n  method: patch\n  operationId: cardPermissionsUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/spend/profiles/{profileId}/cards/{cardToken}/spending-permissions\n  method: patch\n  operationId: cardPermissionsBulkUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /twcard-data/v1/clientSideEncryption/fetchEncryptingKey\n  method: get\n  operationId: cardEncryptionKeyGet\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /twcard-data/v1/sensitive-card-data/details\n  method: post\n  operationId: cardSensitiveDetailsGet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /twcard-data/v1/sensitive-card-data/pin\n  method: post\n  operationId: cardPinGet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/spend/profiles/{profileId}/cards/{cardToken}/phone-number\n  method: put\n  operationId: cardPhoneNumberUpdate\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/spend/profiles/{profileId}/cards/{cardToken}/production\n  method: put\n  operationId: cardKioskCollectionProduce\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/spend/profiles/{profileId}/cards/{cardToken}/production\n  method: get\n  operationId: cardKioskCollectionProductionGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/spend/profiles/{profileId}/card-orders\n\
  \  method: post\n  operationId: cardOrderCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/spend/profiles/{profileId}/card-orders\n  method: get\n  operationId: cardOrderList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/spend/profiles/{profileId}/card-orders/{cardOrderId}\n  method: get\n  operationId: cardOrderGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/spend/profiles/{profileId}/card-orders/availability\n  method: get\n  operationId: cardOrderProgramsGet\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/spend/profiles/{profileId}/card-orders/{cardOrderId}/requirements\n  method: get\n  operationId: cardOrderRequirementsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/spend/profiles/{profileId}/card-orders/{cardOrderId}/status\n  method: put\n  operationId: cardOrderStatusUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/spend/address/validate\n  method: post\n  operationId: cardOrderValidateAddress\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /twcard-data/v1/sensitive-card-data/preset-pin\n  method: post\n  operationId: cardOrderPresetPin\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v3/spend/profiles/{profileId}/cards/transactions/{transactionId}\n  method: get\n  operationId: cardTransactionGetV3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/spend/profiles/{profileId}/cards/transactions/{transactionId}\n\
  \  method: get\n  operationId: cardTransactionGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/spend/profiles/{profileId}/cards/{cardToken}/transactions\n  method: get\n  operationId: cardTransactionList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/user/claim-account\n  method: post\n  operationId: claimAccountCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/comparisons\n  method: get\n  operationId: comparisonGetV3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /v4/comparisons\n  method: get\n  operationId: comparisonGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/profiles/{profileId}/contacts\n  method: post\n  operationId: contactCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/currencies\n  method: get\n  operationId: currenciesGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/delivery-estimates/{transferId}\n  method: get\n  operationId: deliveryEstimateGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/profiles/{profileId}/direct-debit-accounts\n  method: post\n  operationId: directDebitAccountCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/profiles/{profileId}/direct-debit-accounts\n  method: get\n  operationId: directDebitAccountGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/spend/profiles/{profileId}/dispute-form/flows/step/{scheme}/{reason}\n  method: post\n  operationId: disputeDynamicFlowStep\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/spend/profiles/{profileId}/dispute-form/reasons\n  method: get\n  operationId: disputeReasonsGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/spend/profiles/{profileId}/dispute-form/flows/{scheme}/{reason}\n  method: post\n  operationId: disputeSubmit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v4/spend/profiles/{profileId}/dispute-form/file\n  method: post\n  operationId: disputeFileUpload\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/spend/profiles/{profileId}/disputes\n  method: get\n  operationId: disputeList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/spend/profiles/{profileId}/disputes/{disputeId}\n  method: get\n  operationId: disputeGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v3/spend/profiles/{profileId}/disputes/{disputeId}/status\n  method: put\n  operationId: disputeWithdraw\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v3/spend/profiles/{profileId}/dispute-form/file\n  method: post\n  operationId: disputeFileUploadV3\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/facetec/public-key\n  method: get\n  operationId: facetecPublicKeyGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auth/jose/response/public-keys\n  method: get\n  operationId: joseResponsePublicKeysGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auth/jose/request/public-keys\n  method:\
  \ post\n  operationId: joseRequestPublicKeysCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/jose/playground/jws\n  method: post\n  operationId: josePlaygroundJws\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/jose/playground/jwe\n  method: get\n  operationId: josePlaygroundJweGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/auth/jose/playground/jwe\n  method: post\n  operationId: josePlaygroundJwePost\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/jose/playground/jwe-direct-encryption\n  method: post\n  operationId: josePlaygroundJweDirectEncryption\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/auth/jose/playground/jwsjwe\n  method: post\n  operationId: josePlaygroundJwsJwe\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /v1/profiles/{profileId}/kyc-reviews\n  method: post\n  operationId: kycReviewCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/profiles/{profileId}/kyc-reviews\n  method: get\n  operationId: kycReviewList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/profiles/{profileId}/kyc-reviews/{kycReviewId}\n  method: get\n  operationId: kycReviewGetV1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/profiles/{profileId}/kyc-reviews/{kycReviewId}\n  method: patch\n  operationId: kycReviewRedirectUrlUpdate\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/profiles/{profileId}/kyc-reviews/{kycReviewId}\n  method: get\n  operationId: kycReviewGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/profiles/{profileId}/kyc-requirements/{requirementKey}\n  method: post\n  operationId: kycReviewRequirementSubmit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/borderless-accounts-configuration/profiles/{profileId}/available-currencies\n\
  \  method: get\n  operationId: mcaAvailableCurrenciesGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v2/borderless-accounts-configuration/profiles/{profileId}/payin-currencies\n  method: get\n  operationId: mcaPayinCurrenciesGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/profiles/{profileId}/multi-currency-account\n  method: get\n  operationId: mcaGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v4/multi-currency-account/eligibility\n  method: get\n  operationId: mcaEligibilityGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /oauth/token\n  method:\
  \ post\n  operationId: oauthTokenCreate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/one-time-token/status\n  method: get\n  operationId: ottStatusGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/one-time-token/pin/verify\n  method: post\n  operationId: ottPinVerify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/one-time-token/partner-device-fingerprint/verify\n  method: post\n  operationId: ottDeviceFingerprintVerify\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/one-time-token/facemap/verify\n  method: post\n  operationId: ottFacemapVerify\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/application/users/{userId}/phone-numbers\n  method: get\n  operationId: userSecurityPhoneNumberList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    sub\n\n# --- truncated at 32 KB (76 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/wise/refs/heads/main/agentic-access/wise-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/wise/refs/heads/main/agentic-access/wise-agentic-access.yml
summary_line: 238 operations · 147 acting · 6 human-in-the-loop
tags:
- Payments
- FX
- Cross-Border
- Banking
- Multi-Currency
---
