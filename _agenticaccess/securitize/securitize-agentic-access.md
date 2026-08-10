---
acting_count: 64
action_class_counts:
  acting: 64
  connected: 61
api_specs:
- filename: securitize-apac-api-openapi.yml
  format: yaml
  label: Securitize APAC API
  slug: securitize-apac-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/securitize/refs/heads/main/openapi/securitize-apac-api-openapi.yml
- filename: securitize-domains-api-openapi.yml
  format: yaml
  label: Securitize Domains API
  slug: securitize-domains-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/securitize/refs/heads/main/openapi/securitize-domains-api-openapi.yml
- filename: securitize-health-check-api-openapi.yml
  format: yaml
  label: Securitize Health Check API
  slug: securitize-health-check-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/securitize/refs/heads/main/openapi/securitize-health-check-api-openapi.yml
- filename: securitize-travel-rule-api-openapi.yml
  format: yaml
  label: Securitize Travel Rule API
  slug: securitize-travel-rule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/securitize/refs/heads/main/openapi/securitize-travel-rule-api-openapi.yml
- filename: securitize-webhooks-api-openapi.yml
  format: yaml
  label: Securitize Webhooks API
  slug: securitize-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/securitize/refs/heads/main/openapi/securitize-webhooks-api-openapi.yml
consequence_counts:
  read: 61
  safety-critical: 64
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 64
kind: agentic-access
layout: agentic-access
method: generated
name: Securitize Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/apac/domains/{domainId}/tokens/{tokenId}/bank-deposit-files/detail
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/apac/domains/{domainId}/tokens/{tokenId}/bank-deposit-files/detail
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/domains/{domainId}/configurations/general/investors-area
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/domains/{domainId}/custodians/detail
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/domains/{domainId}/investors/bulk
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/domains/{domainId}/investors/detail
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/domains/{domainId}/investors/send-secid-email
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/domains/{domainId}/investors/{externalId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/domains/{domainId}/investors/{externalId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/domains/{domainId}/investors/{externalId}/accreditation/send-email
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/domains/{domainId}/investors/{externalId}/accreditation/status
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/domains/{domainId}/investors/{externalId}/documents/detail
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/domains/{domainId}/investors/{externalId}/documents/detail
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/domains/{domainId}/investors/{externalId}/investment
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/domains/{domainId}/investors/{externalId}/investment/pledged-amount
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/domains/{domainId}/investors/{externalId}/investment/subscription-agreement-status
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/domains/{domainId}/investors/{externalId}/investment/transactions/detail
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /v1/domains/{domainId}/investors/{externalId}/investment/transactions/detail
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/domains/{domainId}/investors/{externalId}/investment/transactions/detail
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/domains/{domainId}/investors/{externalId}/issuances/detail
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/domains/{domainId}/investors/{externalId}/issuances/detail
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /v1/domains/{domainId}/investors/{externalId}/kyc/status
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /v1/domains/{domainId}/investors/{externalId}/labels/detail
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/domains/{domainId}/investors/{externalId}/labels/detail
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: DELETE
  path: /v1/domains/{domainId}/investors/{externalId}/legal-signers/detail
operation_count: 125
overview: 'Securitize exposes 125 API operations that an AI agent could call, of which 64 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 61 read and 64 safety-critical.


  64 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Securitize
provider_slug: securitize
slug: securitize-agentic-access
source_filename: securitize-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-05'\nmethod: generated\nsource: openapi/securitize-domains-openapi-original.json\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 125\n  by_action_class:\n    connected: 61\n    acting: 64\n  by_consequence:\n    read: 61\n    safety-critical: 64\n  human_in_the_loop_required: 64\noperations:\n- path: /v1/health\n  method: get\n  operationId: AppController_root\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/list\n  method: get\n  operationId: DomainsController_getDomains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/domains/{domainId}/currencies/list\n  method: get\n  operationId: CurrenciesController_getCurrencies\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domainId}/custodians/list\n  method: get\n  operationId: CustodiansController_getCustodians\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domainId}/custodians/detail\n  method: post\n  operationId: CustodiansController_addCustodian\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/investors/list\n\
  \  method: get\n  operationId: InvestorsController_getInvestors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domainId}/investors/{externalId}\n  method: get\n  operationId: InvestorsController_getInvestor\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domainId}/investors/{externalId}\n  method: patch\n  operationId: InvestorsController_editInvestor\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/investors/{externalId}\n  method: delete\n  operationId: InvestorsController_deleteInvestor\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/investors/detail\n  method: post\n  operationId: InvestorsController_addInvestor\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/investors/bulk\n  method: post\n  operationId: InvestorsController_addInvestors\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/investors/send-secid-email\n  method: post\n  operationId: InvestorsController_sendInviteSecIdEmails\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/investors/{externalId}/accreditation/status\n  method: get\n  operationId: AccreditationController_getAccreditationStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domainId}/investors/{externalId}/accreditation/status\n  method: put\n\
  \  operationId: AccreditationController_updateAccreditationStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/investors/{externalId}/accreditation/send-email\n  method: post\n  operationId: AccreditationController_sendAccreditationEmail\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/investors/{externalId}/documents/list\n  method: get\n  operationId: DocumentsController_getInvestorDocuments\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domainId}/investors/{externalId}/documents/detail\n  method: get\n  operationId: DocumentsController_getInvestorDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domainId}/investors/{externalId}/documents/detail\n  method: post\n  operationId: DocumentsController_createInvestorDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/investors/{externalId}/documents/detail\n  method: delete\n  operationId: DocumentsController_deleteInvestorDocument\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/investors/{externalId}/investment\n  method: get\n  operationId: InvestmentController_getInvestment\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domainId}/investors/{externalId}/investment\n  method: post\n  operationId: InvestmentController_createInvestment\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop:\
  \ required\n    audit: required\n- path: /v1/domains/{domainId}/investors/{externalId}/investment/funded-amount\n  method: get\n  operationId: FundedAmountController_getFundedAmount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domainId}/investors/{externalId}/investment/funding-address\n  method: get\n  operationId: FundingAddressController_getFundingAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domainId}/investors/{externalId}/investment/pledged-amount\n  method: get\n  operationId: PledgedAmountController_getPledgedAmount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domainId}/investors/{externalId}/investment/pledged-amount\n\
  \  method: put\n  operationId: PledgedAmountController_updatePledgedAmount\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/investors/{externalId}/investment/subscription-agreement-status\n  method: get\n  operationId: SubscriptionAgreementStatusController_getSubscriptionAgreementStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domainId}/investors/{externalId}/investment/subscription-agreement-status\n  method: put\n  operationId: SubscriptionAgreementStatusController_updateSubscriptionAgreementStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/investors/{externalId}/investment/transactions/list\n  method: get\n  operationId: TransactionsController_getTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domainId}/investors/{externalId}/investment/transactions/detail\n  method: post\n  operationId: TransactionsController_createTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n\
  - path: /v1/domains/{domainId}/investors/{externalId}/investment/transactions/detail\n  method: patch\n  operationId: TransactionsController_updateTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/investors/{externalId}/investment/transactions/detail\n  method: delete\n  operationId: TransactionsController_deleteTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/investors/{externalId}/issuances/list\n\
  \  method: get\n  operationId: IssuancesController_getIssuances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domainId}/investors/{externalId}/issuances/detail\n  method: post\n  operationId: IssuancesController_createIssuance\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/investors/{externalId}/issuances/detail\n  method: delete\n  operationId: IssuancesController_deleteIssuance\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/investors/{externalId}/kyc/status\n  method: get\n  operationId: KycController_getKycStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domainId}/investors/{externalId}/kyc/status\n  method: put\n  operationId: KycController_updateKycStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/investors/{externalId}/qualification/status\n  method: get\n  operationId: QualificationController_getQualificationStatus\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domainId}/investors/{externalId}/qualification/status\n  method: put\n  operationId: QualificationController_updateQualificationStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/investors/{externalId}/token-info\n  method: get\n  operationId: TokenInfoController_getTokenInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domainId}/investors/{externalId}/token-info\n  method: patch\n  operationId: TokenInfoController_updateTokenInfo\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/investors/{externalId}/token-wallets/list\n  method: get\n  operationId: TokenWalletsController_getTokenWallets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domainId}/investors/{externalId}/token-wallets/detail\n  method: post\n  operationId: TokenWalletsController_addTokenWallet\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/investors/{externalId}/token-wallets/detail\n  method: patch\n  operationId: TokenWalletsController_updateTokenWallet\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/investors/{externalId}/token-wallets/detail\n  method: delete\n  operationId: TokenWalletsController_deleteTokenWallet\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/investors/{externalId}/labels/list\n\
  \  method: get\n  operationId: LabelsController_getLabels\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domainId}/investors/{externalId}/labels/detail\n  method: post\n  operationId: LabelsController_addLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/investors/{externalId}/labels/detail\n  method: delete\n  operationId: LabelsController_deleteLabel\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession:\
  \ true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/investors/{externalId}/legal-signers/list\n  method: get\n  operationId: LegalSignersController_getLegalSigners\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domainId}/investors/{externalId}/legal-signers/detail\n  method: get\n  operationId: LegalSignersController_getLegalSigner\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domainId}/investors/{externalId}/legal-signers/detail\n  method: delete\n  operationId: LegalSignersController_deleteLegalSigner\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/investors/{externalId}/legal-signers/individual\n  method: post\n  operationId: LegalSignersController_createIndividualLegalSigner\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/investors/{externalId}/legal-signers/entity\n  method: post\n  operationId: LegalSignersController_createEntityLegalSigner\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n\
  \      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/investors/{externalId}/transfer-tbe\n  method: post\n  operationId: TransferTbeController_createTransferTbeTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/investors/{externalId}/token-qualification/status\n  method: get\n  operationId: TokenQualificationController_getTokenQualificationStatus\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domainId}/investors/{externalId}/token-qualification/status\n  method: put\n  operationId: TokenQualificationController_updateTokenQualificationStatus\n\
  \  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/tokens/list\n  method: get\n  operationId: TokensController_getTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domainId}/tokens/{tokenId}\n  method: get\n  operationId: TokensController_getToken\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domainId}/tokens/{tokenId}\n  method: patch\n  operationId: TokensController_updateToken\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/tokens/{tokenId}/nav\n  method: post\n  operationId: TokensController_setNav\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/tokens/{tokenId}/blockchain-transactions/list\n  method: get\n  operationId: BlockchainTransactionsController_getBlockchainTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domainId}/tokens/{tokenId}/blockchain-transactions/detail\n\
  \  method: delete\n  operationId: BlockchainTransactionsController_deleteBlockchainTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/tokens/{tokenId}/blockchain-transactions/detail\n  method: get\n  operationId: BlockchainTransactionsController_getTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domainId}/tokens/{tokenId}/blockchain-transactions/prepare\n  method: post\n  operationId: BlockchainTransactionsController_addBlockchainTransactionData\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience:\
  \ null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/tokens/{tokenId}/blockchain-transactions/send\n  method: post\n  operationId: BlockchainTransactionsController_addBlockchainTransactionSign\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/tokens/{tokenId}/blockchain-transactions/status\n  method: put\n  operationId: BlockchainTransactionsController_updateTransactionStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl:\
  \ 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/tokens/{tokenId}/blockchain-transactions/procedures/lost-shares\n  method: post\n  operationId: ProceduresController_createLostSharesTransactions\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/tokens/{tokenId}/blockchain-transactions/procedures/clawback\n  method: post\n  operationId: ProceduresController_createClawbackTransactions\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange:\
  \ true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/tokens/{tokenId}/blockchain-transactions/procedures/destroy\n  method: post\n  operationId: ProceduresController_createDestroyTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/tokens/{tokenId}/blockchain-transactions/procedures/hold-trading\n  method: post\n  operationId: ProceduresController_createHoldTradingTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/tokens/{tokenId}/blockchain-transactions/procedures/destroy-tbe\n  method: post\n  operationId: ProceduresController_createDestroyTbeTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/tokens/{tokenId}/blockchain-transactions/procedures/internal-transfer-tbe\n  method: post\n  operationId: ProceduresController_createInternalTransferTbeTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/tokens/{tokenId}/documents/list\n  method: get\n  operationId: DocumentsController_getTokenDocuments\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domainId}/tokens/{tokenId}/documents/detail\n  method: get\n  operationId: DocumentsController_getTokenDocument\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domainId}/tokens/{tokenId}/documents/detail\n  method: post\n  operationId: DocumentsController_addTokenDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required:\
  \ true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/tokens/{tokenId}/documents/detail\n  method: patch\n  operationId: DocumentsController_updateTokenDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/tokens/{tokenId}/documents/detail\n  method: delete\n  operationId: DocumentsController_deleteTokenDocument\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n\
  \    audit: required\n- path: /v1/domains/{domainId}/tokens/{tokenId}/holders/list\n  method: get\n  operationId: HoldersController_getHolders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domainId}/tokens/{tokenId}/rounds/list\n  method: get\n  operationId: RoundsController_getRounds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domainId}/tokens/{tokenId}/rounds/detail\n  method: get\n  operationId: RoundsController_getRound\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domainId}/tokens/{tokenId}/rounds/detail\n  method: patch\n  operationId: RoundsController_updateRound\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/tokens/{tokenId}/outreach/notifications/send\n  method: post\n  operationId: NotificationsController_sendNotifications\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-critical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 120\n      exchange: true\n      purpose-required: true\n      proof-of-possession: true\n    escalation:\n      human-in-the-loop: required\n    audit: required\n- path: /v1/domains/{domainId}/tokens/{tokenId}/fundraise/investors/list\n  method: get\n  operationId: FundraiseController_getFundraiseInvestors\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /v1/domains/{domainId}/tokens/{tokenId}/token-transactions/list\n  method: get\n  operationId: TokenTransactionsController_getTokenTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domainId}/tokens/{tokenId}/token-transactions/detail\n  method: get\n  operationId: TokenTransactionsController_getTokenTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domainId}/questions/list\n  method: get\n  operationId: QuestionsController_getQuestions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domainId}/configurations/main-currency\n  method: get\n  operationId: ConfigurationsController_getMainCurrency\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domainId}/configurations/general\n  method: get\n  operationId: GeneralController_getGeneral\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /v1/domains/{domainId}/configurations/general/investors-area\n  method: patch\n  operationId: GeneralController_updateInvestorsArea\n  x-agentic-access:\n    action-class: acting\n    consequence: safety-crit\n\n# --- truncated at 32 KB (44 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/securitize/refs/heads/main/agentic-access/securitize-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/securitize/refs/heads/main/agentic-access/securitize-agentic-access.yml
summary_line: 125 operations · 64 acting · 64 human-in-the-loop
tags:
- tokenization
- digital-securities
- real-world-assets
- capital-markets
- fund-administration
- transfer-agent
- kyc
- aml
- identity-verification
- blockchain
- broker-dealer
- private-credit
- mcp
- webhooks
---
