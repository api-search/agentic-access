---
acting_count: 31
action_class_counts:
  acting: 31
  connected: 38
api_specs:
- filename: unstoppable-finance-addresses-api-openapi.yml
  format: yaml
  label: Unstoppable Finance (Iron) Addresses API
  slug: unstoppable-finance-addresses-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unstoppable-finance/refs/heads/main/openapi/unstoppable-finance-addresses-api-openapi.yml
- filename: unstoppable-finance-autoramp-api-openapi.yml
  format: yaml
  label: Unstoppable Finance (Iron) Autoramp API
  slug: unstoppable-finance-autoramp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unstoppable-finance/refs/heads/main/openapi/unstoppable-finance-autoramp-api-openapi.yml
- filename: unstoppable-finance-currencies-api-openapi.yml
  format: yaml
  label: Unstoppable Finance (Iron) Currencies API
  slug: unstoppable-finance-currencies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unstoppable-finance/refs/heads/main/openapi/unstoppable-finance-currencies-api-openapi.yml
- filename: unstoppable-finance-customer-api-openapi.yml
  format: yaml
  label: Unstoppable Finance (Iron) Customer API
  slug: unstoppable-finance-customer-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unstoppable-finance/refs/heads/main/openapi/unstoppable-finance-customer-api-openapi.yml
- filename: unstoppable-finance-sandbox-api-openapi.yml
  format: yaml
  label: Unstoppable Finance (Iron) Sandbox API
  slug: unstoppable-finance-sandbox-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unstoppable-finance/refs/heads/main/openapi/unstoppable-finance-sandbox-api-openapi.yml
- filename: unstoppable-finance-webhooks-api-openapi.yml
  format: yaml
  label: Unstoppable Finance (Iron) Webhooks API
  slug: unstoppable-finance-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unstoppable-finance/refs/heads/main/openapi/unstoppable-finance-webhooks-api-openapi.yml
- filename: unstoppable-finance-exchange-rate-api-openapi.yml
  format: yaml
  label: Unstoppable Finance (Iron) Exchange Rate API
  slug: unstoppable-finance-exchange-rate-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unstoppable-finance/refs/heads/main/openapi/unstoppable-finance-exchange-rate-api-openapi.yml
- filename: unstoppable-finance-fee-profiles-api-openapi.yml
  format: yaml
  label: Unstoppable Finance (Iron) Fee Profiles API
  slug: unstoppable-finance-fee-profiles-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unstoppable-finance/refs/heads/main/openapi/unstoppable-finance-fee-profiles-api-openapi.yml
- filename: unstoppable-finance-terms-and-conditions-api-openapi.yml
  format: yaml
  label: Unstoppable Finance (Iron) Terms And Conditions API
  slug: unstoppable-finance-terms-and-conditions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/unstoppable-finance/refs/heads/main/openapi/unstoppable-finance-terms-and-conditions-api-openapi.yml
consequence_counts:
  physical: 1
  read: 38
  safety-critical: 2
  write: 28
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 2
kind: agentic-access
layout: agentic-access
method: generated
name: Unstoppable Finance Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /addresses/crypto/{id}/disabled
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /sandbox/reset
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /autoramps/{autoramp_id}/payments/open-banking
operation_count: 69
overview: 'Unstoppable Finance (Iron) exposes 69 API operations that an AI agent could call, of which 31 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 38 read, 28 write, 1 physical, and 2 safety-critical.


  2 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Unstoppable Finance (Iron)
provider_slug: unstoppable-finance
slug: unstoppable-finance-agentic-access
source_filename: unstoppable-finance-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-12'\nmethod: generated\nsource: openapi/unstoppable-finance-addresses-api-openapi.yml, openapi/unstoppable-finance-autoramp-api-openapi.yml,\n  openapi/unstoppable-finance-currencies-api-openapi.yml, openapi/unstoppable-finance-customer-api-openapi.yml,\n  openapi/unstoppable-finance-exchange-rate-api-openapi.yml, openapi/unstoppable-finance-fee-profiles-api-openapi.yml,\n  openapi/unstoppable-finance-sandbox-api-openapi.yml, openapi/unstoppable-finance-terms-and-conditions-api-openapi.yml,\n  openapi/unstoppable-finance-webhooks-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 69\n  by_action_class:\n    acting: 31\n    connected: 38\n  by_consequence:\n    write: 28\n    read: 38\n    safety-critical: 2\n\
  \    physical: 1\n  human_in_the_loop_required: 2\noperations:\n- path: /addresses/crypto/attested\n  method: post\n  operationId: registerAttestedWalletAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /addresses/crypto/hosted\n  method: post\n  operationId: registerHostedWallet\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /addresses/crypto/hosted/vasps\n  method: get\n  operationId: searchHostedVasps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /addresses/crypto/selfhosted\n  method: post\n  operationId: registerSelfHostedWalletAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /addresses/crypto/{customer_id}\n  method: get\n  operationId: getWalletAddresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /addresses/crypto/{id}/disabled\n  method: put\n  operationId: updateDisabledStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /addresses/fiat\n  method: get\n  operationId: getFiatAddressesByStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /addresses/fiat\n  method: post\n  operationId: registerFiatAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /addresses/fiat/{customer_id}\n  method: get\n  operationId: getFiatAddresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /addresses/fiat/{customer_id}/{fiat_address_id}\n  method: delete\n  operationId: deleteFiatAddress\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /addresses/fiat/{customer_id}/{fiat_address_id}\n  method: get\n  operationId: getFiatAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /addresses/fiat/{id}/retry-auth\n  method: post\n  operationId: retryFiatAddressAuth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /addresses/pix\n  method: post\n  operationId: registerPixAddress\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /addresses/pix/{customer_id}\n  method: get\n  operationId: getPixAddresses\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /addresses/pix/{customer_id}/{pix_address_id}\n  method: delete\n  operationId: deletePixAddress\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /addresses/pix/{customer_id}/{pix_address_id}\n  method: get\n  operationId: getPixAddress\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /country_subdivisions/{country_code}\n  method: get\n  operationId: getCountrySubdivisions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autoramp-transactions\n  method: get\n  operationId: getAutorampTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autoramp-transactions/ids\n  method: get\n  operationId: getAutorampTransactionsByIds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autoramps\n  method: get\n  operationId: getAutoramps\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /autoramps\n  method: post\n  operationId: createAutoramp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /autoramps/check-limit\n  method: get\n  operationId: checkAutorampLimit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autoramps/payments/open-banking/{payment_id}\n  method: get\n  operationId: getAutorampOpenBankingPayment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autoramps/quote\n  method: get\n  operationId: getAutorampQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autoramps/quotes-preview\n  method: get\n  operationId: getAutorampQuotePreview\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autoramps/{autoramp_id}\n  method: delete\n  operationId: cancelAutoramp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /autoramps/{autoramp_id}\n  method: get\n  operationId: getAutorampById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autoramps/{autoramp_id}\n  method: patch\n  operationId: patchAutorampMarketById\n  x-agentic-access:\n  \
  \  action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /autoramps/{autoramp_id}/payments/open-banking\n  method: get\n  operationId: listAutorampOpenBankingPayments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autoramps/{autoramp_id}/payments/open-banking\n  method: post\n  operationId: createAutorampOpenBankingPayment\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /autoramps/{autoramp_id}/quote\n\
  \  method: get\n  operationId: getAutorampRateQuote\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /autoramps/{autoramp_id}/quotes\n  method: post\n  operationId: attachQuoteToAutoramp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /autoramps/{autoramp_id}/retry-auth\n  method: post\n  operationId: retryAutorampAuth\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /autoramps/{external_id}/external\n  method: get\n\
  \  operationId: getAutorampByExternalId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /cryptocurrencies\n  method: get\n  operationId: listCryptoCurrencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fiatcurrencies\n  method: get\n  operationId: listFiatCurrencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authentication-codes/entity/{id}\n  method: get\n  operationId: getPendingAuthenticationCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /authentication-codes/{id}\n  method: put\n  operationId: submitAuthenticationCode\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers\n  method: get\n  operationId: getAllCustomers\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers\n  method: post\n  operationId: createCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{external_id}/external\n  method: get\n  operationId: getCustomerByExternalId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n\
  \      max-ttl: 3600\n    audit: none\n- path: /customers/{id}\n  method: get\n  operationId: getCustomerById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}\n  method: put\n  operationId: updateCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{id}/abilities\n  method: get\n  operationId: getCustomerAbilities\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}/archive\n  method: put\n  operationId: archiveCustomer\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject:\
  \ required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{id}/identifications\n  method: get\n  operationId: getAllCustomerIdentifications\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}/identifications/v2\n  method: post\n  operationId: createCustomerIdentificationV2\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{id}/microdeposits\n  method: get\n  operationId: getCustomerMicrodeposits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}/required-signings\n  method: get\n  operationId: getCustomerRequiredSignings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}/requirements\n  method: get\n  operationId: getCustomerRequirements\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}/signings\n  method: get\n  operationId: getSignings\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /customers/{id}/signings\n  method: post\n  operationId: createCustomerSigning\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /customers/{id}/spending-limit\n  method: get\n  operationId: getCustomerSpendingLimit\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /identifications/{id}\n  method: get\n  operationId: getIdentificationById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /identifications/{id}/archive\n  method: put\n  operationId: archiveIdentification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /identifications/{id}/compliance-questionnaire\n\
  \  method: get\n  operationId: getIdentificationComplianceQuestionnaire\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exchange-rate\n  method: get\n  operationId: getExchangeRate\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fee-profiles\n  method: get\n  operationId: getFeeProfiles\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fee-profiles\n  method: post\n  operationId: createFeeProfile\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n\
  - path: /sandbox/autoramp/{id}\n  method: put\n  operationId: updateSandboxAutorampStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sandbox/fiat-verification/{id}\n  method: put\n  operationId: updateSandboxFiatAddressVerificationStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sandbox/identification/{id}\n  method: post\n  operationId: updateSandboxIdentificationStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sandbox/reset\n  method: post\n  operationId: resetSandbox\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /sandbox/transaction\n  method: post\n  operationId: createSandboxTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /sandbox/transaction/{id}/state\n  method: put\n  operationId: updateSandboxTransactionState\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /terms-and-conditions\n  method: get\n  operationId: getAllCurrentTermsAndConditions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks\n  method: get\n  operationId: listWebhooks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /webhooks/{id}\n  method: patch\n  operationId: updateWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n    \
  \  - abnormal\n      - high-value\n    audit: required\n- path: /webhooks/{id}/ping\n  method: post\n  operationId: pingWebhook\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/unstoppable-finance/refs/heads/main/agentic-access/unstoppable-finance-agentic-access.yml
summary_line: 69 operations · 31 acting · 2 human-in-the-loop
tags:
- Company
- Stablecoins
- Payments
- On-Ramp
- Off-Ramp
- Cryptocurrency
- Banking
- Fintech
- Compliance
---
