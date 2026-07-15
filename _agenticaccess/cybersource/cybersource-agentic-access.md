---
acting_count: 120
action_class_counts:
  acting: 120
  connected: 63
api_specs:
- filename: index.html
  format: yaml
  label: CyberSource Payments API
  slug: cybersource-payments-api
  spec_type: OpenAPI
  url: https://developer.cybersource.com/api-reference-assets/index.html
consequence_counts:
  physical: 49
  read: 63
  write: 71
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Cybersource Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /acp/v1/instructions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /acp/v1/instructions/{instructionId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /acp/v1/instructions/{instructionId}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /acp/v1/instructions/{instructionId}/credentials
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /acp/v1/mpp/credentials
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /flex/v2/sessions
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /invoicing/v2/invoiceSettings
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoicing/v2/invoices
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /invoicing/v2/invoices/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoicing/v2/invoices/{id}/cancelation
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoicing/v2/invoices/{id}/delivery
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /invoicing/v2/invoices/{id}/publication
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /ipl/v2/payment-links
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /ipl/v2/payment-links/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pts/v1/pull-funds-transfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pts/v1/pull-funds-transfer/{id}/refund
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pts/v1/pull-funds-transfer/{id}/reversal
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pts/v1/push-funds-transfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pts/v2/captures/{id}/refunds
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pts/v2/intents
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /pts/v2/intents/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pts/v2/payment-references
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /pts/v2/payment-references/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pts/v2/payment-references/{id}/intents
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /pts/v2/payment-tokens
operation_count: 183
overview: 'CyberSource exposes 183 API operations that an AI agent could call, of which 120 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 63 read, 71 write, and 49 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: CyberSource
provider_slug: cybersource
slug: cybersource-agentic-access
source_filename: cybersource-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 183\n  by_action_class:\n    acting: 120\n    connected: 63\n  by_consequence:\n    physical: 49\n    write: 71\n    read: 63\n  human_in_the_loop_required: 0\noperations:\n- path: /pts/v2/payments\n  method: post\n  operationId: createPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pts/v2/payments/{id}\n  method: patch\n  operationId:\
  \ incrementAuth\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pts/v2/payments/{id}/reversals\n  method: post\n  operationId: authReversal\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pts/v2/reversals\n  method: post\n  operationId: mitReversal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pts/v2/payments/{id}/captures\n  method: post\n  operationId: capturePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pts/v2/payments/{id}/refunds\n  method: post\n  operationId: refundPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pts/v2/captures/{id}/refunds\n  method:\
  \ post\n  operationId: refundCapture\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pts/v2/credits\n  method: post\n  operationId: createCredit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pts/v2/payments/{id}/voids\n  method: post\n  operationId: voidPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pts/v2/captures/{id}/voids\n  method: post\n  operationId: voidCapture\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pts/v2/refunds/{id}/voids\n  method: post\n  operationId: voidRefund\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pts/v2/credits/{id}/voids\n  method: post\n  operationId: voidCredit\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pts/v2/voids\n  method: post\n  operationId: mitVoid\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pts/v1/transaction-batches\n  method: get\n  operationId: getTransactionBatches\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pts/v1/transaction-batches/{id}\n  method: get\n  operationId: getTransactionBatchId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pts/v1/transaction-batch-details/{id}\n  method: get\n  operationId: getTransactionBatchDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /pts/v1/transaction-batch-upload\n  method: post\n  operationId: uploadTransactionBatch\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pts/v2/refresh-payment-status/{id}\n  method: post\n  operationId: refreshPaymentStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pts/v2/billing-agreements\n  method: post\n  operationId: billingAgreementsRegistration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pts/v2/billing-agreements/{id}\n  method: patch\n  operationId: billingAgreementsDeRegistration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pts/v2/billing-agreements/{id}/intimations\n  method: post\n  operationId: billingAgreementsIntimation\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pts/v2/payment-references/{id}/intents\n  method: post\n  operationId: createOrderRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pts/v2/payment-references\n  method: post\n  operationId: CreateSessionRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pts/v2/payment-references/{id}\n  method: patch\n  operationId: UpdateSessionReq\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pts/v2/intents\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pts/v2/intents/{id}\n  method: patch\n\
  \  operationId: updateOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pts/v2/payment-tokens\n  method: post\n  operationId: retrieveOrDeletePaymentToken\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tms/v2/tokenize\n  method: post\n  operationId: tokenize\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tms/v2/tokenized-cards\n  method: post\n  operationId: postTokenizedCard\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tms/v2/tokenized-cards/{tokenizedCardId}\n  method: get\n  operationId: getTokenizedCard\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tms/v2/tokenized-cards/{tokenizedCardId}/delete\n  method: post\n  operationId: postTokenizedCardDelete\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n  \
  \  escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tms/v3/tokens/{tokenId}/payment-credentials\n  method: post\n  operationId: postTokenPaymentCredentialsV3\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tms/v2/tokens/{tokenId}/payment-credentials\n  method: post\n  operationId: postTokenPaymentCredentials\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /tms/v2/tokens/{instrumentIdentifierId}/{tokenProvider}/assets/{assetType}\n  method: get\n  operationId: getCardArtAsset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tms/v2/tokenized-cards/{tokenizedCardId}/issuer-life-cycle-event-simulations\n  method: post\n  operationId: postIssuerLifeCycleSimulation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tms/v1/instrumentidentifiers\n  method: post\n  operationId: postInstrumentIdentifier\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tms/v1/instrumentidentifiers/{instrumentIdentifierId}\n  method: get\n  operationId: getInstrumentIdentifier\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tms/v1/instrumentidentifiers/{instrumentIdentifierId}\n  method: patch\n  operationId: patchInstrumentIdentifier\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tms/v1/instrumentidentifiers/{instrumentIdentifierId}\n  method: delete\n  operationId: deleteInstrumentIdentifier\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tms/v1/instrumentidentifiers/{instrumentIdentifierId}/paymentinstruments\n  method: get\n  operationId: getInstrumentIdentifierPaymentInstrumentsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tms/v1/instrumentidentifiers/{instrumentIdentifierId}/enrollment\n  method: post\n  operationId: postInstrumentIdentifierEnrollment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tms/v1/paymentinstruments\n  method: post\n  operationId: postPaymentInstrument\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tms/v1/paymentinstruments/{paymentInstrumentId}\n  method: get\n  operationId: getPaymentInstrument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tms/v1/paymentinstruments/{paymentInstrumentId}\n  method: patch\n  operationId: patchPaymentInstrument\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n     \
  \ - high-value\n    audit: required\n- path: /tms/v1/paymentinstruments/{paymentInstrumentId}\n  method: delete\n  operationId: deletePaymentInstrument\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tms/v2/customers\n  method: post\n  operationId: postCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tms/v2/customers/{customerId}\n  method: get\n  operationId: getCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tms/v2/customers/{customerId}\n  method: patch\n  operationId: patchCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tms/v2/customers/{customerId}\n  method: delete\n  operationId: deleteCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tms/v2/customers/{customerId}/shipping-addresses\n  method: post\n  operationId: postCustomerShippingAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tms/v2/customers/{customerId}/shipping-addresses\n  method: get\n  operationId: getCustomerShippingAddressesList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tms/v2/customers/{customerId}/shipping-addresses/{shippingAddressId}\n  method: get\n  operationId: getCustomerShippingAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tms/v2/customers/{customerId}/shipping-addresses/{shippingAddressId}\n  method: patch\n  operationId: patchCustomersShippingAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tms/v2/customers/{customerId}/shipping-addresses/{shippingAddressId}\n  method: delete\n  operationId: deleteCustomerShippingAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tms/v2/customers/{customerId}/payment-instruments\n  method: post\n  operationId: postCustomerPaymentInstrument\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tms/v2/customers/{customerId}/payment-instruments\n  method: get\n  operationId: getCustomerPaymentInstrumentsList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tms/v2/customers/{customerId}/payment-instruments/{paymentInstrumentId}\n  method: get\n  operationId: getCustomerPaymentInstrument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tms/v2/customers/{customerId}/payment-instruments/{paymentInstrumentId}\n  method: patch\n  operationId: patchCustomersPaymentInstrument\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tms/v2/customers/{customerId}/payment-instruments/{paymentInstrumentId}\n  method: delete\n  operationId: deleteCustomerPaymentInstrument\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /microform/v2/sessions\n  method: post\n  operationId: generateCaptureContext\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /flex/v2/sessions\n  method: post\n  operationId: generateFlexAPICaptureContext\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /risk/v1/decisions\n  method: post\n  operationId: createBundledDecisionManagerCase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /risk/v1/authentication-setups\n  method: post\n  operationId: payerAuthSetup\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /risk/v1/authentications\n  method: post\n  operationId: checkPayerAuthEnrollment\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /risk/v1/authentication-results\n  method: post\n  operationId: validateAuthenticationResults\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /risk/v1/lists/{type}/entries\n\
  \  method: post\n  operationId: addNegative\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /risk/v1/decisions/{id}/actions\n  method: post\n  operationId: actionDecisionManagerCase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /risk/v1/decisions/{id}/comments\n  method: post\n  operationId: commentDecisionManagerCase\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /risk/v1/decisions/{id}/marking\n  method: post\n  operationId: fraudUpdate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /risk/v1/address-verifications\n  method: post\n  operationId: verifyCustomerAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /risk/v1/export-compliance-inquiries\n  method: post\n  operationId: validateExportCompliance\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pts/v2/payouts\n  method: post\n  operationId: octCreatePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pts/v1/push-funds-transfer\n  method: post\n  operationId: createPushFundsTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit:\
  \ required\n- path: /pts/v1/pull-funds-transfer\n  method: post\n  operationId: createPullFundsTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pts/v1/pull-funds-transfer/{id}/reversal\n  method: post\n  operationId: createPullFundsReversal\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /pts/v1/pull-funds-transfer/{id}/refund\n  method: post\n  operationId: createPullFundsRefund\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rbs/v1/plans\n  method: post\n  operationId: createPlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rbs/v1/plans\n  method: get\n  operationId: getPlans\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rbs/v1/plans/{id}\n  method: get\n  operationId: getPlan\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rbs/v1/plans/{id}\n  method: patch\n  operationId: updatePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rbs/v1/plans/{id}\n  method: delete\n  operationId: deletePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rbs/v1/plans/{id}/activate\n  method: post\n  operationId: activatePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rbs/v1/plans/{id}/deactivate\n  method: post\n  operationId: deactivatePlan\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rbs/v1/plans/code\n  method: get\n  operationId: getPlanCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rbs/v1/subscriptions\n  method: post\n  operationId: createSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n    \
  \  triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rbs/v1/subscriptions\n  method: get\n  operationId: getAllSubscriptions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rbs/v1/subscriptions/{id}\n  method: get\n  operationId: getSubscription\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /rbs/v1/subscriptions/{id}\n  method: patch\n  operationId: updateSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rbs/v1/subscriptions/{id}/cancel\n  method: post\n  operationId: cancelSubscription\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rbs/v1/subscriptions/{id}/suspend\n  method: post\n  operationId: suspendSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /rbs/v1/subscriptions/{id}/activate\n  method: post\n  operationId: activateSubscription\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /rbs/v1/subscriptions/code\n  method: get\n  operationId: getSubscriptionCode\n  x-agentic-access:\n    action-class: connecte\n\n# --- truncated at 32 KB (59 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/cybersource/refs/heads/main/agentic-access/cybersource-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/cybersource/refs/heads/main/agentic-access/cybersource-agentic-access.yml
summary_line: 183 operations · 120 acting
tags:
- Payments
- Payment Processing
- Fraud Management
- Tokenization
- Recurring Billing
- Payouts
- Payment Gateway
- Financial Technology
---
