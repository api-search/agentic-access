---
acting_count: 68
action_class_counts:
  acting: 68
  connected: 96
api_specs:
- filename: dwolla-accounts-openapi.yml
  format: yaml
  label: Dwolla Accounts API
  slug: dwolla-accounts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dwolla/refs/heads/main/openapi/dwolla-accounts-openapi.yml
- filename: dwolla-customers-openapi.yml
  format: yaml
  label: Dwolla Customers API
  slug: dwolla-customers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dwolla/refs/heads/main/openapi/dwolla-customers-openapi.yml
- filename: dwolla-beneficial-owners-openapi.yml
  format: yaml
  label: Dwolla Beneficial Owners API
  slug: dwolla-beneficial-owners-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dwolla/refs/heads/main/openapi/dwolla-beneficial-owners-openapi.yml
- filename: dwolla-kba-openapi.yml
  format: yaml
  label: Dwolla KBA API
  slug: dwolla-kba-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dwolla/refs/heads/main/openapi/dwolla-kba-openapi.yml
- filename: dwolla-documents-openapi.yml
  format: yaml
  label: Dwolla Documents API
  slug: dwolla-documents-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dwolla/refs/heads/main/openapi/dwolla-documents-openapi.yml
- filename: dwolla-funding-sources-openapi.yml
  format: yaml
  label: Dwolla Funding Sources API
  slug: dwolla-funding-sources-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dwolla/refs/heads/main/openapi/dwolla-funding-sources-openapi.yml
- filename: dwolla-transfers-openapi.yml
  format: yaml
  label: Dwolla Transfers API
  slug: dwolla-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dwolla/refs/heads/main/openapi/dwolla-transfers-openapi.yml
- filename: dwolla-mass-payments-openapi.yml
  format: yaml
  label: Dwolla Mass Payments API
  slug: dwolla-mass-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dwolla/refs/heads/main/openapi/dwolla-mass-payments-openapi.yml
- filename: dwolla-labels-openapi.yml
  format: yaml
  label: Dwolla Labels API
  slug: dwolla-labels-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dwolla/refs/heads/main/openapi/dwolla-labels-openapi.yml
- filename: dwolla-exchanges-openapi.yml
  format: yaml
  label: Dwolla Exchanges API
  slug: dwolla-exchanges-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dwolla/refs/heads/main/openapi/dwolla-exchanges-openapi.yml
- filename: dwolla-exchange-sessions-openapi.yml
  format: yaml
  label: Dwolla Exchange Sessions API
  slug: dwolla-exchange-sessions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dwolla/refs/heads/main/openapi/dwolla-exchange-sessions-openapi.yml
- filename: dwolla-events-openapi.yml
  format: yaml
  label: Dwolla Events API
  slug: dwolla-events-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dwolla/refs/heads/main/openapi/dwolla-events-openapi.yml
- filename: dwolla-webhook-subscriptions-openapi.yml
  format: yaml
  label: Dwolla Webhook Subscriptions API
  slug: dwolla-webhook-subscriptions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dwolla/refs/heads/main/openapi/dwolla-webhook-subscriptions-openapi.yml
- filename: dwolla-webhooks-openapi.yml
  format: yaml
  label: Dwolla Webhooks API
  slug: dwolla-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dwolla/refs/heads/main/openapi/dwolla-webhooks-openapi.yml
- filename: dwolla-client-tokens-openapi.yml
  format: yaml
  label: Dwolla Client Tokens API
  slug: dwolla-client-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dwolla/refs/heads/main/openapi/dwolla-client-tokens-openapi.yml
- filename: dwolla-tokens-openapi.yml
  format: yaml
  label: Dwolla Tokens API
  slug: dwolla-tokens-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dwolla/refs/heads/main/openapi/dwolla-tokens-openapi.yml
- filename: dwolla-root-openapi.yml
  format: yaml
  label: Dwolla Root API
  slug: dwolla-root-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dwolla/refs/heads/main/openapi/dwolla-root-openapi.yml
- filename: dwolla-sandbox-simulations-openapi.yml
  format: yaml
  label: Dwolla Sandbox Simulations API
  slug: dwolla-sandbox-simulations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dwolla/refs/heads/main/openapi/dwolla-sandbox-simulations-openapi.yml
- filename: dwolla-openapi.yml
  format: yaml
  label: Dwolla API
  slug: dwolla-openapi
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/dwolla/refs/heads/main/openapi/dwolla-openapi.yml
consequence_counts:
  physical: 16
  read: 96
  write: 52
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Dwolla Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /customers/{id}/beneficial-ownership
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /customers/{id}/beneficial-ownership
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /funding-sources/{id}/micro-deposits
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /funding-sources/{id}/micro-deposits
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /mass-payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /mass-payments
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /mass-payments/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /mass-payments/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /on-demand-authorizations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /on-demand-authorizations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sandbox-simulations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /sandbox-simulations
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transfers/{id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /transfers/{id}
operation_count: 164
overview: 'Dwolla exposes 164 API operations that an AI agent could call, of which 68 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 96 read, 52 write, and 16 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Dwolla
provider_slug: dwolla
slug: dwolla-agentic-access
source_filename: dwolla-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-23'\nmethod: generated\nsource: openapi/dwolla-accounts-openapi.yml, openapi/dwolla-beneficial-owners-openapi.yml, openapi/dwolla-client-tokens-openapi.yml,\n  openapi/dwolla-customers-openapi.yml, openapi/dwolla-documents-openapi.yml, openapi/dwolla-events-openapi.yml,\n  openapi/dwolla-exchange-sessions-openapi.yml, openapi/dwolla-exchanges-openapi.yml, openapi/dwolla-funding-sources-openapi.yml,\n  openapi/dwolla-kba-openapi.yml, openapi/dwolla-labels-openapi.yml, openapi/dwolla-mass-payments-openapi.yml,\n  openapi/dwolla-openapi.yml, openapi/dwolla-root-openapi.yml, openapi/dwolla-sandbox-simulations-openapi.yml,\n  openapi/dwolla-tokens-openapi.yml, openapi/dwolla-transfers-openapi.yml, openapi/dwolla-webhook-subscriptions-openapi.yml,\n  openapi/dwolla-webhooks-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review\
  \ and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 164\n  by_action_class:\n    connected: 96\n    acting: 68\n  by_consequence:\n    read: 96\n    write: 52\n    physical: 16\n  human_in_the_loop_required: 0\noperations:\n- path: /accounts/{id}\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /funding-sources\n  method: post\n  operationId: createFundingSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{id}/funding-sources\n  method: get\n  operationId: listFundingSources\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{id}/transfers\n  method: get\n  operationId: listAndSearchTransfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{id}/mass-payments\n  method: get\n  operationId: listMassPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}/beneficial-owners\n  method: get\n  operationId: listBeneficialOwnersForCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}/beneficial-owners\n  method: post\n  operationId: createBeneficialOwnerForCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n\
  \    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /beneficial-owners/{id}\n  method: get\n  operationId: retrieveBeneficialOwner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /beneficial-owners/{id}\n  method: post\n  operationId: updateBeneficialOwner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /beneficial-owners/{id}\n  method: delete\n  operationId: deleteBeneficialOwner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n  \
  \    max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{id}/beneficial-ownership\n  method: get\n  operationId: getBeneficialOwnershipStatusForCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}/beneficial-ownership\n  method: post\n  operationId: certifyBeneficialOwnershipForCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /client-tokens\n  method: post\n  operationId: createClientToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers\n  method: get\n  operationId: listAndSearchCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers\n  method: post\n  operationId: createCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{id}\n  method: get\n  operationId: getCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}\n\
  \  method: post\n  operationId: update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /business-classifications\n  method: get\n  operationId: listBusinessClassifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /business-classifications/{id}\n  method: get\n  operationId: retrieveBusinessClassification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}/documents\n  method: get\n  operationId: listCustomerDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /customers/{id}/documents\n  method: post\n  operationId: createCustomerDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /beneficial-owners/{id}/documents\n  method: get\n  operationId: listBeneficialOwnerDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /beneficial-owners/{id}/documents\n  method: post\n  operationId: createBeneficialOwnerDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n   \
  \   - high-value\n    audit: required\n- path: /documents/{id}\n  method: get\n  operationId: retrieveDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events\n  method: get\n  operationId: listEvents\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /events/{id}\n  method: get\n  operationId: getEvent\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}/exchange-sessions\n  method: post\n  operationId: createCustomerExchangeSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n     \
  \ - abnormal\n      - high-value\n    audit: required\n- path: /exchange-sessions/{id}\n  method: get\n  operationId: retrieveCustomerExchangeSession\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exchanges/{id}/exchange-sessions\n  method: post\n  operationId: createReAuthExchangeSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{id}/available-exchange-connections\n  method: get\n  operationId: listAvailableExchangeConnections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exchange-partners\n  method: get\n  operationId:\
  \ listExchangePartners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exchange-partners/{id}\n  method: get\n  operationId: getExchangePartner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exchanges\n  method: get\n  operationId: listAccountExchanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exchanges\n  method: post\n  operationId: createAccountExchange\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /exchanges/{id}\n  method:\
  \ get\n  operationId: getExchange\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}/exchanges\n  method: get\n  operationId: listCustomerExchanges\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}/exchanges\n  method: post\n  operationId: createCustomerExchange\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{id}/funding-sources\n  method: get\n  operationId: listCustomerFundingSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /customers/{id}/funding-sources\n  method: post\n  operationId: createCustomerFundingSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /funding-sources/{id}\n  method: get\n  operationId: getFundingSource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /funding-sources/{id}\n  method: post\n  operationId: updateOrRemoveFundingSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /funding-sources/{id}/micro-deposits\n  method: get\n  operationId: getMicroDeposits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /funding-sources/{id}/micro-deposits\n  method: post\n  operationId: initiateOrVerifyMicroDeposits\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /funding-sources/{id}/balance\n  method: get\n  operationId: getFundingSourceBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /funding-sources/{id}/ach-routing\n  method: get\n  operationId: getVanRouting\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /on-demand-authorizations\n  method: post\n  operationId: createOnDemandTransferAuthorization\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{id}/kba\n  method: post\n  operationId: initiateKbaForCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /kba/{id}\n  method: get\n  operationId: getKbaQuestions\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /kba/{id}\n  method: post\n  operationId: verifyKbaQuestions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /labels/{id}\n  method: get\n  operationId: getLabel\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /labels/{id}\n  method: delete\n  operationId: removeLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n\
  \      - high-value\n    audit: required\n- path: /customers/{id}/labels\n  method: get\n  operationId: listCustomerLabels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}/labels\n  method: post\n  operationId: createCustomerLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /labels/{id}/ledger-entries\n  method: get\n  operationId: listLabelLedgerEntries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /labels/{id}/ledger-entries\n  method: post\n  operationId: createLabelLedgerEntry\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /ledger-entries/{ledgerEntryId}\n  method: get\n  operationId: getLabelLedgerEntry\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /label-reallocations\n  method: post\n  operationId: createLabelReallocation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /label-reallocations/{reallocationId}\n  method: get\n  operationId: retrieveLabelReallocation\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mass-payments\n  method: post\n  operationId: initiateMassPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mass-payments/{id}\n  method: get\n  operationId: getMassPayment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mass-payments/{id}\n  method: post\n  operationId: updateMassPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mass-payments/{id}/items\n  method: get\n  operationId: listMassPaymentItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mass-payment-items/{itemId}\n  method: get\n  operationId: getMassPaymentItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}/mass-payments\n  method: get\n  operationId: listCustomerMassPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /token\n  method: post\n  operationId: createApplicationAccessToken\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /\n  method: get\n  operationId: getRoot\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{id}\n  method: get\n  operationId: getAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /funding-sources\n  method: post\n  operationId: createFundingSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /accounts/{id}/funding-sources\n  method: get\n  operationId:\
  \ listFundingSources\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{id}/transfers\n  method: get\n  operationId: listAndSearchTransfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /accounts/{id}/mass-payments\n  method: get\n  operationId: listMassPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers\n  method: get\n  operationId: listAndSearchCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers\n  method: post\n  operationId: createCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{id}\n  method: get\n  operationId: getCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}\n  method: post\n  operationId: update\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /business-classifications\n  method: get\n  operationId: listBusinessClassifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /business-classifications/{id}\n\
  \  method: get\n  operationId: retrieveBusinessClassification\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}/beneficial-owners\n  method: get\n  operationId: listBeneficialOwnersForCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}/beneficial-owners\n  method: post\n  operationId: createBeneficialOwnerForCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /beneficial-owners/{id}\n  method: get\n  operationId: retrieveBeneficialOwner\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /beneficial-owners/{id}\n  method: post\n  operationId: updateBeneficialOwner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /beneficial-owners/{id}\n  method: delete\n  operationId: deleteBeneficialOwner\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{id}/beneficial-ownership\n  method: get\n  operationId: getBeneficialOwnershipStatusForCustomer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}/beneficial-ownership\n  method: post\n  operationId: certifyBeneficialOwnershipForCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{id}/documents\n  method: get\n  operationId: listCustomerDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}/documents\n  method: post\n  operationId: createCustomerDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /beneficial-owners/{id}/documents\n  method: get\n  operationId: listBeneficialOwnerDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /beneficial-owners/{id}/documents\n  method: post\n  operationId: createBeneficialOwnerDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /documents/{id}\n  method: get\n  operationId: retrieveDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}/kba\n  method:\
  \ post\n  operationId: initiateKbaForCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /kba/{id}\n  method: get\n  operationId: getKbaQuestions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /kba/{id}\n  method: post\n  operationId: verifyKbaQuestions\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{id}/funding-sources\n  method: get\n  operationId: listCustomerFundingSources\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}/funding-sources\n  method: post\n  operationId: createCustomerFundingSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /funding-sources/{id}\n  method: get\n  operationId: getFundingSource\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /funding-sources/{id}\n  method: post\n  operationId: updateOrRemoveFundingSource\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /funding-sources/{id}/micro-deposits\n  method: get\n  operationId: getMicroDeposits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /funding-sources/{id}/micro-deposits\n  method: post\n  operationId: initiateOrVerifyMicroDeposits\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /funding-sources/{id}/balance\n  method: get\n  operationId: getFundingSourceBalance\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /funding-sources/{id}/ach-routing\n  method: get\n  operationId: getVanRouting\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /on-demand-authorizations\n  method: post\n  operationId: createOnDemandTransferAuthorization\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transfers\n  method: post\n  operationId: initiateTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /transfers/{id}\n  method: get\n  operationId: getTransfer\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transfers/{id}\n  method: post\n  operationId: cancelTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{id}/transfers\n  method: get\n  operationId: listCustomerTransfers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transfers/{id}/fees\n  method: get\n  operationId: listTransferFees\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transfers/{id}/failure\n  method: get\n  operationId: getTransferFailureReason\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mass-payments\n  method: post\n  operationId: initiateMassPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mass-payments/{id}\n  method: get\n  operationId: getMassPayment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /mass-payments/{id}\n  method: post\n  operationId: updateMassPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /mass-payments/{id}/items\n  method: get\n  operationId: listMassPaymentItems\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /mass-payment-items/{itemId}\n  method: get\n  operationId: getMassPaymentItem\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}/mass-payments\n  method: get\n  operationId: listCustomerMassPayments\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit\n\n# --- truncated at 32 KB (45 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/dwolla/refs/heads/main/agentic-access/dwolla-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/dwolla/refs/heads/main/agentic-access/dwolla-agentic-access.yml
summary_line: 164 operations · 68 acting
tags:
- Payments
- ACH
- Bank Transfers
- Fintech
- Account-to-Account Payments
- Money Movement
- Instant Payments
- Open Banking
- Webhooks
- KYC
- United States
- Open Finance
- Same-Day ACH
- RTP
- FedNow
- Mass Payments
- Drop-in Components
- SDKs
- Sandbox
---
