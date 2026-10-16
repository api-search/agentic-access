---
acting_count: 25
action_class_counts:
  acting: 25
  connected: 32
api_specs:
- filename: openpayments-io-account-information-service-ais-api-openapi.yml
  format: yaml
  label: Open Payments Account Information Service (AIS) API
  slug: openpayments-io-account-information-service-ais-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-account-information-service-ais-api-openapi.yml
- filename: openpayments-io-aspsp-information-service-api-openapi.yml
  format: yaml
  label: Open Payments ASPSP Information Service API
  slug: openpayments-io-aspsp-information-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-aspsp-information-service-api-openapi.yml
- filename: openpayments-io-bankgiro-lookup-api-openapi.yml
  format: yaml
  label: Open Payments Bankgiro Lookup API
  slug: openpayments-io-bankgiro-lookup-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-bankgiro-lookup-api-openapi.yml
- filename: openpayments-io-consent-service-api-openapi.yml
  format: yaml
  label: Open Payments Consent Service API
  slug: openpayments-io-consent-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-consent-service-api-openapi.yml
- filename: openpayments-io-fx-connect-api-openapi.yml
  format: yaml
  label: Open Payments FX Connect API
  slug: openpayments-io-fx-connect-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-fx-connect-api-openapi.yml
- filename: openpayments-io-iso-payments-api-openapi.yml
  format: yaml
  label: Open Payments ISO Payments API
  slug: openpayments-io-iso-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-iso-payments-api-openapi.yml
- filename: openpayments-io-kyc-service-api-openapi.yml
  format: yaml
  label: Open Payments KYC Service API
  slug: openpayments-io-kyc-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-kyc-service-api-openapi.yml
- filename: openpayments-io-payment-initiation-service-pis-api-openapi.yml
  format: yaml
  label: Open Payments Payment Initiation Service (PIS) API
  slug: openpayments-io-payment-initiation-service-pis-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-payment-initiation-service-pis-api-openapi.yml
- filename: openpayments-io-payout-service-api-openapi.yml
  format: yaml
  label: Open Payments Payout Service API
  slug: openpayments-io-payout-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-payout-service-api-openapi.yml
- filename: openpayments-io-sepa-direct-debit-api-openapi.yml
  format: yaml
  label: Open Payments SEPA Direct Debit API
  slug: openpayments-io-sepa-direct-debit-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-sepa-direct-debit-api-openapi.yml
- filename: openpayments-io-verification-of-payee-vop-api-openapi.yml
  format: yaml
  label: Open Payments Verification of Payee (VoP) API
  slug: openpayments-io-verification-of-payee-vop-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/openapi/openpayments-io-verification-of-payee-vop-api-openapi.yml
consequence_counts:
  physical: 18
  read: 32
  write: 7
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Openpayments Io Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /iso/beta/payments/sepa-direct-debit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /iso/payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /iso/payments/confirm
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /iso/payments/cross-border
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /premium/v1/payouts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /premium/v1/payouts/confirm
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /psd2/paymentinitiation/v1/fx
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /psd2/paymentinitiation/v1/fx/{fxQuoteId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /psd2/paymentinitiation/v1/signing-baskets
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /psd2/paymentinitiation/v1/signing-baskets/{basketId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /psd2/paymentinitiation/v1/signing-baskets/{basketId}/authorisations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /psd2/paymentinitiation/v1/signing-baskets/{basketId}/authorisations/{authorisationId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /psd2/paymentinitiation/v1/{payment-service}/{payment-product}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /psd2/paymentinitiation/v1/{payment-service}/{payment-product}/{paymentId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /psd2/paymentinitiation/v1/{payment-service}/{payment-product}/{paymentId}/authorisations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /psd2/paymentinitiation/v1/{payment-service}/{payment-product}/{paymentId}/authorisations/{authorisationId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /psd2/paymentinitiation/v1/{payment-service}/{payment-product}/{paymentId}/cancellation-authorisations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /psd2/paymentinitiation/v1/{payment-service}/{payment-product}/{paymentId}/cancellation-authorisations/{cancellationId}
operation_count: 57
overview: 'Open Payments exposes 57 API operations that an AI agent could call, of which 25 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 32 read, 7 write, and 18 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Open Payments
provider_slug: openpayments-io
slug: openpayments-io-agentic-access
source_filename: openpayments-io-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-15'\nmethod: generated\nsource: openapi/openpayments-io-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 57\n  by_action_class:\n    acting: 25\n    connected: 32\n  by_consequence:\n    write: 7\n    read: 32\n    physical: 18\n  human_in_the_loop_required: 0\noperations:\n- path: /premium/v1/payee-verifications\n  method: post\n  operationId: Submit Verification of Payee\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - paymentinitiation corporate\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /premium/v1/bulk-payee-verifications\n\
  \  method: post\n  operationId: Submit Bulk Verification of Payee\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - paymentinitiation corporate\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /premium/v1/creditor-name\n  method: get\n  operationId: Get Creditor Name\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - paymentinitiation corporate\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /premium/v1/giro-numbers\n  method: get\n  operationId: Get Giro Numbers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - paymentinitiation corporate\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iso/payments\n  method: post\n  operationId: Create\
  \ Payment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - paymentinitiation corporate\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iso/payments/cross-border\n  method: post\n  operationId: Create Payment (Cross-Border)\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - paymentinitiation corporate\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iso/beta/payments/sepa-direct-debit\n  method: post\n  operationId: Create SEPA Direct Debit Payment\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - paymentinitiation corporate\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /iso/payments/{paymentId}\n  method: get\n  operationId: Get Payment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - paymentinitiation corporate\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /iso/payments/confirm\n  method: put\n  operationId: Confirm Payment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - paymentinitiation corporate\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /premium/v1/payouts\n  method: post\n  operationId: Create Payout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - paymentinitiation corporate\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /premium/v1/payouts/{payoutId}\n  method: get\n  operationId: Get Payout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - paymentinitiation corporate\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /premium/v1/payouts/confirm\n  method: put\n  operationId: Confirm Payout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n \
  \   - paymentinitiation corporate\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /kyc/integration/v1/new/{PSU-Corporate-ID}\n  method: post\n  operationId: new\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - paymentinitiation corporate\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /kyc/integration/v1/status/{PSU-Corporate-ID}\n  method: get\n  operationId: status\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - paymentinitiation corporate\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /psd2/paymentinitiation/v1/{payment-service}/{payment-product}\n\
  \  method: post\n  operationId: initiatePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - paymentinitiation corporate\n    - paymentinitiation private\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /psd2/paymentinitiation/v1/{payment-service}/{payment-product}/{paymentId}\n  method: get\n  operationId: getPaymentInformation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - paymentinitiation corporate\n    - paymentinitiation private\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /psd2/paymentinitiation/v1/{payment-service}/{payment-product}/{paymentId}\n  method: delete\n  operationId: cancelPayment\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: physical\n    subject: required\n    scope:\n    - paymentinitiation corporate\n    - paymentinitiation private\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /psd2/paymentinitiation/v1/{payment-service}/{payment-product}/{paymentId}/status\n  method: get\n  operationId: getPaymentInitiationStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - paymentinitiation corporate\n    - paymentinitiation private\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /psd2/paymentinitiation/v1/{payment-service}/{payment-product}/{paymentId}/authorisations\n  method: post\n  operationId: startPaymentAuthorisation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n\
  \    - paymentinitiation corporate\n    - paymentinitiation private\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /psd2/paymentinitiation/v1/{payment-service}/{payment-product}/{paymentId}/authorisations\n  method: get\n  operationId: getPaymentInitiationAuthorisation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - paymentinitiation corporate\n    - paymentinitiation private\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /psd2/paymentinitiation/v1/{payment-service}/{payment-product}/{paymentId}/authorisations/{authorisationId}\n  method: get\n  operationId: getPaymentInitiationScaStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - paymentinitiation\
  \ corporate\n    - paymentinitiation private\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /psd2/paymentinitiation/v1/{payment-service}/{payment-product}/{paymentId}/authorisations/{authorisationId}\n  method: put\n  operationId: updatePaymentPsuData\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - paymentinitiation corporate\n    - paymentinitiation private\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /psd2/paymentinitiation/v1/{payment-service}/{payment-product}/{paymentId}/cancellation-authorisations\n  method: post\n  operationId: startPaymentInitiationCancellationAuthorisation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - paymentinitiation\
  \ corporate\n    - paymentinitiation private\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /psd2/paymentinitiation/v1/{payment-service}/{payment-product}/{paymentId}/cancellation-authorisations\n  method: get\n  operationId: getPaymentInitiationCancellationAuthorisationInformation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - paymentinitiation corporate\n    - paymentinitiation private\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /psd2/paymentinitiation/v1/{payment-service}/{payment-product}/{paymentId}/cancellation-authorisations/{cancellationId}\n  method: get\n  operationId: getPaymentCancellationScaStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n\
  \    - paymentinitiation corporate\n    - paymentinitiation private\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /psd2/paymentinitiation/v1/{payment-service}/{payment-product}/{paymentId}/cancellation-authorisations/{cancellationId}\n  method: put\n  operationId: updatePaymentCancellationPsuData\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - paymentinitiation corporate\n    - paymentinitiation private\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /psd2/paymentinitiation/v1/signing-baskets\n  method: post\n  operationId: createSigningBasket\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - paymentinitiation corporate\n    - paymentinitiation private\n\
  \    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /psd2/paymentinitiation/v1/signing-baskets/{basketId}\n  method: get\n  operationId: getSigningBasket\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - paymentinitiation corporate\n    - paymentinitiation private\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /psd2/paymentinitiation/v1/signing-baskets/{basketId}\n  method: delete\n  operationId: deleteSigningBasket\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - paymentinitiation corporate\n    - paymentinitiation private\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /psd2/paymentinitiation/v1/signing-baskets/{basketId}/status\n  method: get\n  operationId: getSigningBasketStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - paymentinitiation corporate\n    - paymentinitiation private\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /psd2/paymentinitiation/v1/signing-baskets/{basketId}/authorisations\n  method: post\n  operationId: startSigningBasketAuthorisation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - paymentinitiation corporate\n    - paymentinitiation private\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /psd2/paymentinitiation/v1/signing-baskets/{basketId}/authorisations/{authorisationId}\n  method: put\n  operationId: updateSigningBasketPsuData\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - paymentinitiation corporate\n    - paymentinitiation private\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /psd2/paymentinitiation/v1/signing-baskets/{basketId}/authorisations/{authorisationId}\n  method: get\n  operationId: getSigningBasketScaStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - paymentinitiation corporate\n    - paymentinitiation private\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /psd2/paymentinitiation/v1/fx\n  method: post\n  operationId:\
  \ createFxQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - paymentinitiation corporate\n    - paymentinitiation private\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /psd2/paymentinitiation/v1/fx/{fxQuoteId}\n  method: get\n  operationId: getFxQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - paymentinitiation corporate\n    - paymentinitiation private\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /psd2/paymentinitiation/v1/fx/{fxQuoteId}\n  method: put\n  operationId: confirmCrossBorderPaymentIntent\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    scope:\n    - paymentinitiation corporate\n\
  \    - paymentinitiation private\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /psd2/accountinformation/v1/accounts\n  method: get\n  operationId: getAccountList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accountinformation bankgiroinformation corporate\n    - accountinformation corporate\n    - accountinformation private\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /psd2/accountinformation/v1/accounts/{account-id}\n  method: get\n  operationId: readAccountDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accountinformation bankgiroinformation corporate\n    - accountinformation corporate\n    - accountinformation private\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /psd2/accountinformation/v1/accounts/{account-id}/balances\n  method: get\n  operationId: getBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accountinformation bankgiroinformation corporate\n    - accountinformation corporate\n    - accountinformation private\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /psd2/accountinformation/v1/accounts/{account-id}/transactions\n  method: get\n  operationId: getTransactionList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accountinformation bankgiroinformation corporate\n    - accountinformation corporate\n    - accountinformation private\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /psd2/accountinformation/v1/accounts/{account-id}/transactions/{transactionId}\n  method: get\n  operationId: getTransactionDetails\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accountinformation bankgiroinformation corporate\n    - accountinformation corporate\n    - accountinformation private\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /psd2/accountinformation/v1/card-accounts\n  method: get\n  operationId: getCardAccountList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accountinformation corporate\n    - accountinformation private\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /psd2/accountinformation/v1/card-accounts/{account-id}\n  method: get\n  operationId: readCardAccountDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accountinformation corporate\n    - accountinformation private\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /psd2/accountinformation/v1/card-accounts/{account-id}/balances\n\
  \  method: get\n  operationId: getCardBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accountinformation corporate\n    - accountinformation private\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /psd2/accountinformation/v1/card-accounts/{account-id}/transactions\n  method: get\n  operationId: getCardTransactionList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accountinformation corporate\n    - accountinformation private\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /psd2/consent/v1/consents\n  method: post\n  operationId: createConsent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accountinformation bankgiroinformation corporate\n    - accountinformation corporate\n    - accountinformation private\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /psd2/consent/v1/consents/{consentId}\n  method: get\n  operationId: getConsentInformation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accountinformation bankgiroinformation corporate\n    - accountinformation corporate\n    - accountinformation private\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /psd2/consent/v1/consents/{consentId}\n  method: delete\n  operationId: deleteConsent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accountinformation bankgiroinformation corporate\n    - accountinformation corporate\n    - accountinformation private\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /psd2/consent/v1/consents/{consentId}/status\n  method: get\n  operationId: getConsentStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accountinformation bankgiroinformation corporate\n    - accountinformation corporate\n    - accountinformation private\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /psd2/consent/v1/consents/{consentId}/authorisations\n  method: post\n  operationId: startConsentAuthorisation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    - accountinformation bankgiroinformation corporate\n    - accountinformation corporate\n    - accountinformation private\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /psd2/consent/v1/consents/{consentId}/authorisations\n\
  \  method: get\n  operationId: getConsentAuthorisation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accountinformation bankgiroinformation corporate\n    - accountinformation corporate\n    - accountinformation private\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /psd2/consent/v1/consents/{consentId}/authorisations/{authorisationId}\n  method: get\n  operationId: getConsentScaStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accountinformation bankgiroinformation corporate\n    - accountinformation corporate\n    - accountinformation private\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /psd2/consent/v1/consents/{consentId}/authorisations/{authorisationId}\n  method: put\n  operationId: updateConsentsPsuData\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    scope:\n    -\
  \ accountinformation bankgiroinformation corporate\n    - accountinformation corporate\n    - accountinformation private\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /psd2/aspspinformation/v1/aspsps\n  method: get\n  operationId: getASPSPList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - aspspinformation corporate\n    - aspspinformation private\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /psd2/aspspinformation/v1/aspsps/{bicFi}\n  method: get\n  operationId: getASPSPDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - aspspinformation corporate\n    - aspspinformation private\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /psd2/aspspinformation/v1/countries\n  method: get\n  operationId:\
  \ getCountriesList\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - aspspinformation corporate\n    - aspspinformation private\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/status\n  method: get\n  operationId: getObpStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    scope:\n    - accountinformation corporate\n    - accountinformation private\n    - paymentinitiation corporate\n    - paymentinitiation private\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/openpayments-io/refs/heads/main/agentic-access/openpayments-io-agentic-access.yml
summary_line: 57 operations · 25 acting
tags:
- Company
- Payments
- Banking
- API
- FinTech
---
