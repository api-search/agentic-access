---
acting_count: 50
action_class_counts:
  acting: 50
  connected: 51
api_specs:
- filename: triodos-bank-uk-account-information-service-api-openapi.yml
  format: yaml
  label: Triodos Bank UK Account Information Service API
  slug: triodos-bank-uk-account-information-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triodos-bank-uk/refs/heads/main/openapi/triodos-bank-uk-account-information-service-api-openapi.yml
- filename: triodos-bank-uk-authorization-endpoint-api-openapi.yml
  format: yaml
  label: Triodos Bank UK Authorization Endpoint API
  slug: triodos-bank-uk-authorization-endpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triodos-bank-uk/refs/heads/main/openapi/triodos-bank-uk-authorization-endpoint-api-openapi.yml
- filename: triodos-bank-uk-client-registration-endpoint-api-openapi.yml
  format: yaml
  label: Triodos Bank UK Client Registration Endpoint API
  slug: triodos-bank-uk-client-registration-endpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triodos-bank-uk/refs/heads/main/openapi/triodos-bank-uk-client-registration-endpoint-api-openapi.yml
- filename: triodos-bank-uk-configuration-endpoint-api-openapi.yml
  format: yaml
  label: Triodos Bank UK Configuration Endpoint API
  slug: triodos-bank-uk-configuration-endpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triodos-bank-uk/refs/heads/main/openapi/triodos-bank-uk-configuration-endpoint-api-openapi.yml
- filename: triodos-bank-uk-confirmation-of-funds-service-api-openapi.yml
  format: yaml
  label: Triodos Bank UK Confirmation of Funds Service API
  slug: triodos-bank-uk-confirmation-of-funds-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triodos-bank-uk/refs/heads/main/openapi/triodos-bank-uk-confirmation-of-funds-service-api-openapi.yml
- filename: triodos-bank-uk-extended-account-information-service-api-openapi.yml
  format: yaml
  label: Triodos Bank UK Extended Account Information Service API
  slug: triodos-bank-uk-extended-account-information-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triodos-bank-uk/refs/heads/main/openapi/triodos-bank-uk-extended-account-information-service-api-openapi.yml
- filename: triodos-bank-uk-initial-access-token-service-api-openapi.yml
  format: yaml
  label: Triodos Bank UK Initial Access Token Service API
  slug: triodos-bank-uk-initial-access-token-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triodos-bank-uk/refs/heads/main/openapi/triodos-bank-uk-initial-access-token-service-api-openapi.yml
- filename: triodos-bank-uk-payment-initiation-service-api-openapi.yml
  format: yaml
  label: Triodos Bank UK Payment Initiation Service API
  slug: triodos-bank-uk-payment-initiation-service-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triodos-bank-uk/refs/heads/main/openapi/triodos-bank-uk-payment-initiation-service-api-openapi.yml
- filename: triodos-bank-uk-token-endpoint-api-openapi.yml
  format: yaml
  label: Triodos Bank UK Token Endpoint API
  slug: triodos-bank-uk-token-endpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triodos-bank-uk/refs/heads/main/openapi/triodos-bank-uk-token-endpoint-api-openapi.yml
- filename: triodos-bank-uk-userinfo-endpoint-api-openapi.yml
  format: yaml
  label: Triodos Bank UK UserInfo Endpoint API
  slug: triodos-bank-uk-userinfo-endpoint-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/triodos-bank-uk/refs/heads/main/openapi/triodos-bank-uk-userinfo-endpoint-api-openapi.yml
consequence_counts:
  physical: 36
  read: 51
  safety-critical: 1
  write: 13
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 1
kind: agentic-access
layout: agentic-access
method: generated
name: Triodos Bank Uk Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /{tenant}/v1/token/revoke
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{tenant}/v1/bulk-payments/sepa-credit-transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /{tenant}/v1/bulk-payments/sepa-credit-transfers/{resource-id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{tenant}/v1/bulk-payments/sepa-credit-transfers/{resource-id}/authorisations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /{tenant}/v1/bulk-payments/sepa-credit-transfers/{resource-id}/authorisations/{authorisation-id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{tenant}/v1/bulk-payments/sepa-credit-transfers/{resource-id}/cancellation-authorisations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /{tenant}/v1/bulk-payments/sepa-credit-transfers/{resource-id}/cancellation-authorisations/{authorisation-id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{tenant}/v1/payments/cross-border-credit-transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /{tenant}/v1/payments/cross-border-credit-transfers/{resource-id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{tenant}/v1/payments/cross-border-credit-transfers/{resource-id}/authorisations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /{tenant}/v1/payments/cross-border-credit-transfers/{resource-id}/authorisations/{authorisation-id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{tenant}/v1/payments/cross-border-credit-transfers/{resource-id}/cancellation-authorisations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /{tenant}/v1/payments/cross-border-credit-transfers/{resource-id}/cancellation-authorisations/{authorisation-id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{tenant}/v1/payments/sepa-credit-transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /{tenant}/v1/payments/sepa-credit-transfers/{resource-id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{tenant}/v1/payments/sepa-credit-transfers/{resource-id}/authorisations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /{tenant}/v1/payments/sepa-credit-transfers/{resource-id}/authorisations/{authorisation-id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{tenant}/v1/payments/sepa-credit-transfers/{resource-id}/cancellation-authorisations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /{tenant}/v1/payments/sepa-credit-transfers/{resource-id}/cancellation-authorisations/{authorisation-id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{tenant}/v1/payments/uk-domestic-transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /{tenant}/v1/payments/uk-domestic-transfers/{resource-id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{tenant}/v1/payments/uk-domestic-transfers/{resource-id}/authorisations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /{tenant}/v1/payments/uk-domestic-transfers/{resource-id}/authorisations/{authorisation-id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /{tenant}/v1/payments/uk-domestic-transfers/{resource-id}/cancellation-authorisations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /{tenant}/v1/payments/uk-domestic-transfers/{resource-id}/cancellation-authorisations/{authorisation-id}
operation_count: 101
overview: 'Triodos Bank UK exposes 101 API operations that an AI agent could call, of which 50 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 51 read, 13 write, 36 physical, and 1 safety-critical.


  1 operation are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Triodos Bank UK
provider_slug: triodos-bank-uk
slug: triodos-bank-uk-agentic-access
source_filename: triodos-bank-uk-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: generated\nsource: openapi/triodos-bank-uk-auth-openapi.json, openapi/triodos-bank-uk-xs2a-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 101\n  by_action_class:\n    connected: 51\n    acting: 50\n  by_consequence:\n    read: 51\n    write: 13\n    safety-critical: 1\n    physical: 36\n  human_in_the_loop_required: 1\noperations:\n- path: /{tenant}/v1/auth\n  method: get\n  operationId: authorizeGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant}/v1/auth\n  method: post\n  operationId: authorizePost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/.well-known/openid-configuration\n  method: get\n  operationId: configuration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant}/v1/registration\n  method: post\n  operationId: authorizePost_1\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/v1/token\n  method: post\n  operationId: token\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/v1/token/revoke\n  method: post\n  operationId: tokenRevocation\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /{tenant}/v1/userinfo\n  method: get\n  operationId: doGet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant}/v1/userinfo\n  method: post\n  operationId: doPost\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/onboarding/v1\n  method: get\n  operationId: initialAccessToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant}/v1/accounts/{account-id}\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant}/v1/accounts\n  method: get\n  operationId: getAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant}/v1/accounts/{account-id}/balances\n  method: get\n  operationId: getBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n  \
  \  audit: none\n- path: /{tenant}/v1/accounts/{account-id}/transactions\n  method: get\n  operationId: getTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant}/v1/accounts/{account-id}/transactions/page\n  method: get\n  operationId: getTransactionsPage\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant}/v1/bulk-payments/sepa-credit-transfers/{resource-id}/authorisations\n  method: get\n  operationId: getAuthorisations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant}/v1/bulk-payments/sepa-credit-transfers/{resource-id}/authorisations\n  method: post\n  operationId: createAuthorisation\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/v1/bulk-payments/sepa-credit-transfers/{resource-id}/authorisations/{authorisation-id}\n  method: get\n  operationId: getAuthorisation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant}/v1/bulk-payments/sepa-credit-transfers/{resource-id}/authorisations/{authorisation-id}\n  method: put\n  operationId: submitAuthorisation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/v1/bulk-payments/sepa-credit-transfers/{resource-id}/cancellation-authorisations\n  method: get\n  operationId: getCancellationAuthorisations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant}/v1/bulk-payments/sepa-credit-transfers/{resource-id}/cancellation-authorisations\n  method: post\n  operationId: createCancellationAuthorisation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/v1/bulk-payments/sepa-credit-transfers/{resource-id}/cancellation-authorisations/{authorisation-id}\n  method: get\n  operationId:\
  \ getCancellationAuthorisation\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant}/v1/bulk-payments/sepa-credit-transfers/{resource-id}/cancellation-authorisations/{authorisation-id}\n  method: put\n  operationId: submitCancellationAuthorisation\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/v1/bulk-payments/sepa-credit-transfers/{resource-id}\n  method: delete\n  operationId: deletePayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/v1/bulk-payments/sepa-credit-transfers/{resource-id}/status\n  method: get\n  operationId: getStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant}/v1/bulk-payments/sepa-credit-transfers\n  method: post\n  operationId: initiateSepaBulkPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/v1/funds-confirmations\n  method: post\n  operationId: confirmFundsAvailable\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/v1/consents/{resource-id}/authorisations\n  method: get\n  operationId: getAisAuthorisations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant}/v1/consents/{resource-id}/authorisations\n  method: post\n  operationId: createAisAuthorisation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/v1/consents/{resource-id}/authorisations/{authorisation-id}\n  method: get\n  operationId: getAisAuthorisationStatus\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant}/v1/consents/{resource-id}/authorisations/{authorisation-id}\n  method: put\n  operationId: submitAisAuthorisation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/v1/consents/{resource-id}\n  method: get\n  operationId: getAisConsent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant}/v1/consents/{resource-id}\n  method: delete\n  operationId: deleteAisConsent\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n\
  \    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/v1/consents/{resource-id}/status\n  method: get\n  operationId: getAisConsentStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant}/v1/consents\n  method: post\n  operationId: registerConsentRequest\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/v1/payments/cross-border-credit-transfers/{resource-id}/authorisations\n  method: get\n  operationId: getAuthorisations_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant}/v1/payments/cross-border-credit-transfers/{resource-id}/authorisations\n  method: post\n  operationId: createAuthorisation_1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/v1/payments/cross-border-credit-transfers/{resource-id}/authorisations/{authorisation-id}\n  method: get\n  operationId: getAuthorisation_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant}/v1/payments/cross-border-credit-transfers/{resource-id}/authorisations/{authorisation-id}\n  method: put\n  operationId: submitAuthorisation_1\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/v1/payments/cross-border-credit-transfers/{resource-id}/cancellation-authorisations\n  method: get\n  operationId: getCancellationAuthorisations_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant}/v1/payments/cross-border-credit-transfers/{resource-id}/cancellation-authorisations\n  method: post\n  operationId: createCancellationAuthorisation_1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required:\
  \ true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/v1/payments/cross-border-credit-transfers/{resource-id}/cancellation-authorisations/{authorisation-id}\n  method: get\n  operationId: getCancellationAuthorisation_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant}/v1/payments/cross-border-credit-transfers/{resource-id}/cancellation-authorisations/{authorisation-id}\n  method: put\n  operationId: submitCancellationAuthorisation_1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/v1/payments/cross-border-credit-transfers/{resource-id}\n\
  \  method: delete\n  operationId: deletePayment_1\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/v1/payments/cross-border-credit-transfers/{resource-id}/status\n  method: get\n  operationId: getStatus_1\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant}/v1/payments/cross-border-credit-transfers\n  method: post\n  operationId: initiateCrossBorderPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/v1/payments/sepa-credit-transfers/{resource-id}/authorisations\n  method: get\n  operationId: getAuthorisations_2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant}/v1/payments/sepa-credit-transfers/{resource-id}/authorisations\n  method: post\n  operationId: createAuthorisation_2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/v1/payments/sepa-credit-transfers/{resource-id}/authorisations/{authorisation-id}\n  method: get\n  operationId: getAuthorisation_2\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant}/v1/payments/sepa-credit-transfers/{resource-id}/authorisations/{authorisation-id}\n  method: put\n  operationId: submitAuthorisation_2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/v1/payments/sepa-credit-transfers/{resource-id}/cancellation-authorisations\n  method: get\n  operationId: getCancellationAuthorisations_2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant}/v1/payments/sepa-credit-transfers/{resource-id}/cancellation-authorisations\n\
  \  method: post\n  operationId: createCancellationAuthorisation_2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/v1/payments/sepa-credit-transfers/{resource-id}/cancellation-authorisations/{authorisation-id}\n  method: get\n  operationId: getCancellationAuthorisation_2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant}/v1/payments/sepa-credit-transfers/{resource-id}/cancellation-authorisations/{authorisation-id}\n  method: put\n  operationId: submitCancellationAuthorisation_2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n  \
  \  audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/v1/payments/sepa-credit-transfers/{resource-id}\n  method: delete\n  operationId: deletePayment_2\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/v1/payments/sepa-credit-transfers/{resource-id}/status\n  method: get\n  operationId: getStatus_2\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant}/v1/payments/sepa-credit-transfers\n\
  \  method: post\n  operationId: initiateSepaPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/v1/payments/uk-domestic-transfers/{resource-id}/authorisations\n  method: get\n  operationId: getAuthorisations_3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant}/v1/payments/uk-domestic-transfers/{resource-id}/authorisations\n  method: post\n  operationId: createAuthorisation_3\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/v1/payments/uk-domestic-transfers/{resource-id}/authorisations/{authorisation-id}\n  method: get\n  operationId: getAuthorisation_3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant}/v1/payments/uk-domestic-transfers/{resource-id}/authorisations/{authorisation-id}\n  method: put\n  operationId: submitAuthorisation_3\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/v1/payments/uk-domestic-transfers/{resource-id}/cancellation-authorisations\n\
  \  method: get\n  operationId: getCancellationAuthorisations_3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant}/v1/payments/uk-domestic-transfers/{resource-id}/cancellation-authorisations\n  method: post\n  operationId: createCancellationAuthorisation_3\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/v1/payments/uk-domestic-transfers/{resource-id}/cancellation-authorisations/{authorisation-id}\n  method: get\n  operationId: getCancellationAuthorisation_3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /{tenant}/v1/payments/uk-domestic-transfers/{resource-id}/cancellation-authorisations/{authorisation-id}\n  method: put\n  operationId: submitCancellationAuthorisation_3\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/v1/payments/uk-domestic-transfers/{resource-id}\n  method: delete\n  operationId: deletePayment_3\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/v1/payments/uk-domestic-transfers/{resource-id}/status\n\
  \  method: get\n  operationId: getStatus_3\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant}/v1/payments/uk-domestic-transfers\n  method: post\n  operationId: initiateUkDomesticPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/v1/periodic-payments/sepa-credit-transfers/{resource-id}/authorisations\n  method: get\n  operationId: getAuthorisations_4\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant}/v1/periodic-payments/sepa-credit-transfers/{resource-id}/authorisations\n\
  \  method: post\n  operationId: createAuthorisation_4\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/v1/periodic-payments/sepa-credit-transfers/{resource-id}/authorisations/{authorisation-id}\n  method: get\n  operationId: getAuthorisation_4\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant}/v1/periodic-payments/sepa-credit-transfers/{resource-id}/authorisations/{authorisation-id}\n  method: put\n  operationId: submitAuthorisation_4\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/v1/periodic-payments/sepa-credit-transfers/{resource-id}/cancellation-authorisations\n  method: get\n  operationId: getCancellationAuthorisations_4\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant}/v1/periodic-payments/sepa-credit-transfers/{resource-id}/cancellation-authorisations\n  method: post\n  operationId: createCancellationAuthorisation_4\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /{tenant}/v1/periodic-payments/sepa-credit-transfers/{resource-id}/cancellation-authorisations/{authorisation-id}\n  method: get\n  operationId: getCancellationAuthorisation_4\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant}/v1/periodic-payments/sepa-credit-transfers/{resource-id}/cancellation-authorisations/{authorisation-id}\n  method: put\n  operationId: submitCancellationAuthorisation_4\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/v1/periodic-payments/sepa-credit-transfers/{resource-id}\n  method: delete\n  operationId: deletePayment_4\n  x-agentic-access:\n \
  \   action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/v1/periodic-payments/sepa-credit-transfers/{resource-id}/status\n  method: get\n  operationId: getStatus_4\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant}/v1/periodic-payments/sepa-credit-transfers\n  method: post\n  operationId: initiateSepaPeriodicPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n   \
  \   - high-value\n    audit: required\n- path: /{tenant}/v1/periodic-payments/uk-domestic-transfers/{resource-id}/authorisations\n  method: get\n  operationId: getAuthorisations_5\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant}/v1/periodic-payments/uk-domestic-transfers/{resource-id}/authorisations\n  method: post\n  operationId: createAuthorisation_5\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/v1/periodic-payments/uk-domestic-transfers/{resource-id}/authorisations/{authorisation-id}\n  method: get\n  operationId: getAuthorisation_5\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant}/v1/periodic-payments/uk-domestic-transfers/{resource-id}/authorisations/{authorisation-id}\n  method: put\n  operationId: submitAuthorisation_5\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/v1/periodic-payments/uk-domestic-transfers/{resource-id}/cancellation-authorisations\n  method: get\n  operationId: getCancellationAuthorisations_5\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant}/v1/periodic-payments/uk-domestic-transfers/{resource-id}/cancellation-authorisations\n\
  \  method: post\n  operationId: createCancellationAuthorisation_5\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/v1/periodic-payments/uk-domestic-transfers/{resource-id}/cancellation-authorisations/{authorisation-id}\n  method: get\n  operationId: getCancellationAuthorisation_5\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant}/v1/periodic-payments/uk-domestic-transfers/{resource-id}/cancellation-authorisations/{authorisation-id}\n  method: put\n  operationId: submitCancellationAuthorisation_5\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/v1/periodic-payments/uk-domestic-transfers/{resource-id}\n  method: delete\n  operationId: deletePayment_5\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/v1/periodic-payments/uk-domestic-transfers/{resource-id}/status\n  method: get\n  operationId: getStatus_5\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant}/v1/periodic-payments/uk-domestic-transfers\n\
  \  method: post\n  operationId: initiateUkDomesticPeriodicPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /{tenant}/v2/consents/confirmation-of-funds/{resource-id}/authorisations\n  method: get\n  operationId: getPiisAuthorisations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /{tenant}/v2/consents/confirmation-of-funds/{resource-id}/authorisations\n\n# --- truncated at 32 KB (35 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/triodos-bank-uk/refs/heads/main/agentic-access/triodos-bank-uk-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/triodos-bank-uk/refs/heads/main/agentic-access/triodos-bank-uk-agentic-access.yml
summary_line: 101 operations · 50 acting · 1 human-in-the-loop
tags:
- Financial-Services
- Banking
- Open Banking
- PSD2
- XS2A
- Berlin Group
- United Kingdom
- Payments
- Account Information
- Confirmation of Funds
- Ethical Banking
- Sustainable Finance
- Specialist Lender
---
