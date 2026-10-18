---
acting_count: 38
action_class_counts:
  acting: 38
  connected: 30
api_specs:
- filename: caliza-beneficiary-v1-api-openapi.yml
  format: yaml
  label: Caliza Beneficiary V1 API
  slug: caliza-beneficiary-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caliza/refs/heads/main/openapi/caliza-beneficiary-v1-api-openapi.yml
- filename: caliza-integrator-capabilities-v1-api-openapi.yml
  format: yaml
  label: Caliza Integrator Capabilities V1 API
  slug: caliza-integrator-capabilities-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caliza/refs/heads/main/openapi/caliza-integrator-capabilities-v1-api-openapi.yml
- filename: caliza-integrator-v1-api-openapi.yml
  format: yaml
  label: Caliza Integrator V1 API
  slug: caliza-integrator-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caliza/refs/heads/main/openapi/caliza-integrator-v1-api-openapi.yml
- filename: caliza-kyc-kyb-v1-api-openapi.yml
  format: yaml
  label: Caliza KYC/KYB V1 API
  slug: caliza-kyc-kyb-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caliza/refs/heads/main/openapi/caliza-kyc-kyb-v1-api-openapi.yml
- filename: caliza-payment-v1-api-openapi.yml
  format: yaml
  label: Caliza Payment V1 API
  slug: caliza-payment-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caliza/refs/heads/main/openapi/caliza-payment-v1-api-openapi.yml
- filename: caliza-recipient-v1-api-openapi.yml
  format: yaml
  label: Caliza Recipient V1 API
  slug: caliza-recipient-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caliza/refs/heads/main/openapi/caliza-recipient-v1-api-openapi.yml
- filename: caliza-related-person-api-openapi.yml
  format: yaml
  label: Caliza Related Person API
  slug: caliza-related-person-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caliza/refs/heads/main/openapi/caliza-related-person-api-openapi.yml
- filename: caliza-terms-and-conditions-v1-api-openapi.yml
  format: yaml
  label: Caliza Terms and Conditions V1 API
  slug: caliza-terms-and-conditions-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caliza/refs/heads/main/openapi/caliza-terms-and-conditions-v1-api-openapi.yml
- filename: caliza-transaction-v1-api-openapi.yml
  format: yaml
  label: Caliza Transaction V1 API
  slug: caliza-transaction-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caliza/refs/heads/main/openapi/caliza-transaction-v1-api-openapi.yml
- filename: caliza-transaction-v1-sandbox-api-openapi.yml
  format: yaml
  label: Caliza Transaction V1 Sandbox API
  slug: caliza-transaction-v1-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caliza/refs/heads/main/openapi/caliza-transaction-v1-sandbox-api-openapi.yml
- filename: caliza-travel-rule-v1-api-openapi.yml
  format: yaml
  label: Caliza Travel Rule V1 API
  slug: caliza-travel-rule-v1-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/caliza/refs/heads/main/openapi/caliza-travel-rule-v1-api-openapi.yml
consequence_counts:
  physical: 14
  read: 30
  safety-critical: 1
  write: 23
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Caliza Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/beneficiaries/{beneficiaryId}/disable
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payments/:withDocuments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/simulations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/transactions/payouts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/transactions/sandbox/crypto-deposit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/transactions/sandbox/pix
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/transactions/sandbox/pixOutConfirmation
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/transactions/sandbox/spei
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/transactions/sandbox/usd-deposit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/transactions/sweep-payouts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/travel-rule/proofs
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/travel-rule/proofs/manual-attestation
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/travel-rule/proofs/microtransfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v2/simulations
operation_count: 68
overview: 'Caliza exposes 68 API operations that an AI agent could call, of which 38 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 30 read, 23 write, 14 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Caliza
provider_slug: caliza
slug: caliza-agentic-access
source_filename: caliza-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-14'\nmethod: generated\nsource: openapi/caliza-api-documentation-reference-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 68\n  by_action_class:\n    connected: 30\n    acting: 38\n  by_consequence:\n    read: 30\n    write: 23\n    safety-critical: 1\n    physical: 14\n  human_in_the_loop_required: 1\noperations:\n- path: /v1/beneficiaries\n  method: get\n  operationId: getAll\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/beneficiaries\n  method: post\n  operationId: saveBeneficiary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/beneficiaries/{beneficiaryId}\n  method: get\n  operationId: getBeneficiary\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/beneficiaries/{beneficiaryId}\n  method: put\n  operationId: updateBeneficiary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/beneficiaries/{beneficiaryId}\n  method: delete\n  operationId: deleteBeneficiary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/beneficiaries/{beneficiaryId}/balances\n  method: get\n  operationId: getBeneficiaryBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/beneficiaries/{beneficiaryId}/balances/details\n  method: get\n  operationId: getBeneficiaryDetailedBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/beneficiaries/{beneficiaryId}/disable\n  method: post\n  operationId: disableBeneficiary\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n\
  \    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/beneficiaries/{beneficiaryId}/enable\n  method: post\n  operationId: enableBeneficiary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/beneficiaries/{beneficiaryId}/multi-currencies-balances/details\n  method: get\n  operationId: getBeneficiaryDetailedBalanceByCurrencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/beneficiaries/{beneficiaryId}/related-persons\n  method: post\n  operationId: createRelatedPerson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/beneficiaries/{beneficiaryId}/related-persons\n  method: get\n  operationId: listRelatedPersons\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/beneficiaries/{beneficiaryId}/related-persons/{id}\n  method: get\n  operationId: getRelatedPerson\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/beneficiaries/{beneficiaryId}/related-persons/{id}\n  method: put\n  operationId: updateRelatedPerson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n   \
  \   - high-value\n    audit: required\n- path: /v1/beneficiaries/{beneficiaryId}/related-persons/{id}\n  method: delete\n  operationId: deleteRelatedPerson\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/beneficiaries/{beneficiaryId}/related-persons/{id}/documents\n  method: post\n  operationId: addRelatedPersonDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/beneficiaries/{beneficiaryId}/terms-and-conditions\n  method: post\n  operationId: acceptTermsAndConditions\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/beneficiaries/{beneficiaryId}/travel-rule/deposit-info\n  method: get\n  operationId: getDepositInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/beneficiaries/{beneficiaryId}/verification\n  method: post\n  operationId: createVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/beneficiaries/{beneficiaryId}/verification\n  method: get\n  operationId: getVerificationStatus\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/beneficiaries/{beneficiaryId}/verification/sandbox/approve\n  method: post\n  operationId: approveVerificationSandbox\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/beneficiaries/{beneficiaryId}/virtualAccounts\n  method: get\n  operationId: listVirtualAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/beneficiaries/{beneficiaryId}/virtualAccounts\n  method: post\n  operationId: createVirtualAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n   \
  \ audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/beneficiaries/{beneficiaryId}/wallets\n  method: get\n  operationId: findOrCreateWallet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/integrator-capabilities\n  method: get\n  operationId: getCapabilitiesByIntegratorId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/integrators/me\n  method: get\n  operationId: getMe\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/integrators/me\n  method: put\n  operationId: updateMe\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/integrators/{integratorId}/balances\n  method: get\n  operationId: getIntegratorBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/integrators/{integratorId}/update-webhook-secret\n  method: post\n  operationId: updateIntegratorWebhookSecret\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/integrators/{integratorId}/webhook-secret\n  method: get\n  operationId: getIntegratorWebhookSecret\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/integrators/{integratorId}/webhooks\n  method: get\n  operationId: getIntegratorWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/integrators/{integratorId}/webhooks\n  method: patch\n  operationId: updateWebhookConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/payments\n  method: post\n  operationId: createPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/payments/:withDocuments\n  method: post\n  operationId: createPaymentWithDocuments\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/payments/payment-instructions\n  method: get\n  operationId: getPaymentInstructions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/payments/{id}\n  method: get\n  operationId: getTransactionById_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n  \
  \    max-ttl: 3600\n    audit: none\n- path: /v1/recipients\n  method: get\n  operationId: getRecipients\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recipients\n  method: post\n  operationId: createRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/recipients/vasps/search\n  method: get\n  operationId: searchVasps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recipients/{id}\n  method: get\n  operationId: getRecipient\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n   \
  \ token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/recipients/{id}\n  method: put\n  operationId: updateRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/recipients/{id}\n  method: delete\n  operationId: deleteRecipient\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/simulations\n  method: post\n  operationId: createSimulation_1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n\
  \      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/simulations/{id}\n  method: get\n  operationId: getSimulationById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/terms-and-conditions\n  method: get\n  operationId: getTermsAndConditions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transactions\n  method: post\n  operationId: createTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transactions\n\
  \  method: get\n  operationId: getAllTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transactions/:withDocuments\n  method: post\n  operationId: createTransaction_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transactions/deposit-instructions\n  method: get\n  operationId: getDepositInstructions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transactions/payouts\n  method: post\n  operationId: payouts\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transactions/sandbox/crypto-deposit\n  method: post\n  operationId: createFakeCryptoDeposit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transactions/sandbox/pix\n  method: post\n  operationId: createFakePixInDeposit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transactions/sandbox/pixOutConfirmation\n  method: post\n  operationId: createFakePixInDeposit_1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transactions/sandbox/spei\n  method: post\n  operationId: createFakeSpeiInDeposit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transactions/sandbox/travel-rule-clearance\n\
  \  method: post\n  operationId: simulateTravelRuleClearance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transactions/sandbox/usd-deposit\n  method: post\n  operationId: createFakeUSDDeposit\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transactions/sweep-payouts\n  method: post\n  operationId: sweepPayouts\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n\
  \      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/transactions/{id}\n  method: get\n  operationId: getTransactionById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transactions/{id}/:withDocuments\n  method: get\n  operationId: getTransactionByIdWithDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/transactions/{id}/documents\n  method: post\n  operationId: uploadDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/transactions/{id}/proof-of-payment\n  method: get\n  operationId: getTransactionProofOfPayment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/travel-rule/proofs\n  method: post\n  operationId: submitProof\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/travel-rule/proofs\n  method: get\n  operationId: getProof\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/travel-rule/proofs/delegate-token\n  method: post\n  operationId: issueDelegateToken\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/travel-rule/proofs/manual-attestation\n  method: post\n  operationId: issueManualAttestation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/travel-rule/proofs/microtransfer\n  method: post\n  operationId: startMicrotransferTest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/simulations\n  method: post\n  operationId: createSimulation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v2/simulations/{id}\n  method: get\n  operationId: getSimulationByIdV2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/caliza/refs/heads/main/agentic-access/caliza-agentic-access.yml
summary_line: 68 operations · 38 acting · 1 human-in-the-loop
tags:
- Company
- Fintech
- Payments
- Cross-Border Payments
- Stablecoins
- Remittances
- Foreign Exchange
- Virtual Accounts
- Payouts
- KYC
- Latin America
---
