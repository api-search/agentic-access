---
acting_count: 30
action_class_counts:
  acting: 30
  connected: 16
api_specs:
- filename: insumermodel-com-agent-commerce-protocols-api-openapi.yml
  format: yaml
  label: insumermodel-com Agent Commerce Protocols API
  slug: insumermodel-com-agent-commerce-protocols-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/insumermodel-com/openapi/insumermodel-com-agent-commerce-protocols-api-openapi.yml
- filename: insumermodel-com-agent-onboarding-api-openapi.yml
  format: yaml
  label: insumermodel-com Agent Onboarding API
  slug: insumermodel-com-agent-onboarding-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/insumermodel-com/openapi/insumermodel-com-agent-onboarding-api-openapi.yml
- filename: insumermodel-com-discounts-codes-api-openapi.yml
  format: yaml
  label: insumermodel-com Discounts & Codes API
  slug: insumermodel-com-discounts-codes-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/insumermodel-com/openapi/insumermodel-com-discounts-codes-api-openapi.yml
- filename: insumermodel-com-discovery-api-openapi.yml
  format: yaml
  label: insumermodel-com Discovery API
  slug: insumermodel-com-discovery-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/insumermodel-com/openapi/insumermodel-com-discovery-api-openapi.yml
- filename: insumermodel-com-keys-billing-api-openapi.yml
  format: yaml
  label: insumermodel-com Keys & Billing API
  slug: insumermodel-com-keys-billing-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/insumermodel-com/openapi/insumermodel-com-keys-billing-api-openapi.yml
- filename: insumermodel-com-merchant-setup-api-openapi.yml
  format: yaml
  label: insumermodel-com Merchant Setup API
  slug: insumermodel-com-merchant-setup-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/insumermodel-com/openapi/insumermodel-com-merchant-setup-api-openapi.yml
- filename: insumermodel-com-platform-api-openapi.yml
  format: yaml
  label: insumermodel-com Platform API
  slug: insumermodel-com-platform-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/insumermodel-com/openapi/insumermodel-com-platform-api-openapi.yml
- filename: insumermodel-com-point-of-sale-api-openapi.yml
  format: yaml
  label: insumermodel-com Point of Sale API
  slug: insumermodel-com-point-of-sale-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/insumermodel-com/openapi/insumermodel-com-point-of-sale-api-openapi.yml
- filename: insumermodel-com-trust-fact-profiles-api-openapi.yml
  format: yaml
  label: insumermodel-com Trust Fact Profiles API
  slug: insumermodel-com-trust-fact-profiles-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/insumermodel-com/openapi/insumermodel-com-trust-fact-profiles-api-openapi.yml
- filename: insumermodel-com-wallet-auth-api-openapi.yml
  format: yaml
  label: insumermodel-com Wallet Auth API
  slug: insumermodel-com-wallet-auth-api
  spec_type: OpenAPI
  url: https://artifacts.apis.io/insumermodel-com/openapi/insumermodel-com-wallet-auth-api-openapi.yml
consequence_counts:
  physical: 4
  read: 16
  write: 26
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Insumermodel Com Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/keys/checkout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/keys/purchase
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /v1/merchants/{id}/verification
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /v1/payment/confirm
operation_count: 46
overview: 'insumermodel-com exposes 46 API operations that an AI agent could call, of which 30 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 16 read, 26 write, and 4 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: insumermodel-com
provider_slug: insumermodel-com
slug: insumermodel-com-agentic-access
source_filename: insumermodel-com-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-10-30'\nmethod: generated\nsource: openapi/insumermodel-com-openapi.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 46\n  by_action_class:\n    connected: 16\n    acting: 30\n  by_consequence:\n    read: 16\n    write: 26\n    physical: 4\n  human_in_the_loop_required: 0\noperations:\n- path: /v1/jwks\n  method: get\n  operationId: getJwks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/compliance/templates\n  method: get\n  operationId: listComplianceTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /v1/attest\n  method: post\n  operationId: createAttestation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/trust\n  method: post\n  operationId: walletTrust\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/trust/batch\n  method: post\n  operationId: batchWalletTrust\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n\
  \    audit: required\n- path: /v1/credits\n  method: get\n  operationId: getCredits\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/keys/buy\n  method: post\n  operationId: buyKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/keys/purchase\n  method: post\n  operationId: purchaseTieredKey\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/credits/buy\n\
  \  method: post\n  operationId: buyCredits\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/merchants\n  method: get\n  operationId: listMerchants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/merchants\n  method: post\n  operationId: createMerchant\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/merchants/{id}\n  method: get\n  operationId: getMerchant\n  x-agentic-access:\n    action-class: connected\n\
  \    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/tokens\n  method: get\n  operationId: listTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/discount/check\n  method: get\n  operationId: checkDiscount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/verify\n  method: post\n  operationId: createVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/payment/confirm\n  method: post\n  operationId: confirmPayment\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/merchants/{id}/tokens\n  method: put\n  operationId: updateMerchantTokens\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/merchants/{id}/nfts\n  method: put\n  operationId: updateMerchantNfts\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path:\
  \ /v1/merchants/{id}/settings\n  method: put\n  operationId: updateMerchantSettings\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/merchants/{id}/credits\n  method: post\n  operationId: buyMerchantCredits\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/merchants/{id}/directory\n  method: post\n  operationId: publishToDirectory\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop:\
  \ conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/merchants/{id}/status\n  method: get\n  operationId: getMerchantStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/merchants/{id}/domain-verification\n  method: post\n  operationId: requestDomainVerification\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/merchants/{id}/domain-verification\n  method: put\n  operationId: verifyDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/merchants/{id}/verification\n  method: put\n  operationId: partnerAssertDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/registry/submit\n  method: post\n  operationId: submitToRegistry\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/merchants/{id}/scanners\n  method: post\n  operationId: manageMerchantScanners\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/merchants/{id}/scanners\n  method: get\n  operationId: listMerchantScanners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/scanner/session\n  method: post\n  operationId: scannerSession\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/pass/verify\n  method: post\n  operationId: verifyPass\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n  \
  \    max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/acp/discount\n  method: post\n  operationId: acpDiscount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/ucp/discount\n  method: post\n  operationId: ucpDiscount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/codes/{code}\n  method: get\n  operationId: validateCode\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/registry/tokens\n  method: get\n  operationId: getRegistryTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/registry/merchants\n  method: get\n  operationId: getRegistryMerchants\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/health\n  method: get\n  operationId: healthCheck\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/keys/create\n  method: post\n  operationId: createFreeKey\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n  \
  \    triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/keys/checkout\n  method: post\n  operationId: createKeyCheckout\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/keys/retrieve\n  method: get\n  operationId: retrieveKeyAfterCheckout\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/keys/lookup\n  method: post\n  operationId: lookupAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/credits/topup\n  method: post\n  operationId: buyCreditsWithCard\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/billing/portal\n  method: post\n  operationId: openBillingPortal\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/chain-request\n  method: post\n  operationId: requestChainSupport\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/merchants/{id}/claims\n\
  \  method: get\n  operationId: listDomainClaims\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/merchants/{id}/claims\n  method: post\n  operationId: resolveDomainClaim\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /v1/merchants/{id}/release\n  method: post\n  operationId: releaseDomain\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n"
source_yaml_url: https://artifacts.apis.io/insumermodel-com/agentic-access/insumermodel-com-agentic-access.yml
summary_line: 46 operations · 30 acting
tags:
- Wallet Auth
- Blockchain
- AI Agents
- Condition-Based Access
- Cryptocurrency
- Developer Tools
---
