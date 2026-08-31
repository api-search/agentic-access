---
acting_count: 24
action_class_counts:
  acting: 24
  connected: 28
api_specs:
- filename: fipto-aisp-pisp-api-openapi.yml
  format: yaml
  label: Fipto AISP/PISP API
  slug: fipto-aisp-pisp-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fipto/refs/heads/main/openapi/fipto-aisp-pisp-api-openapi.yml
- filename: fipto-assets-api-openapi.yml
  format: yaml
  label: Fipto Assets API
  slug: fipto-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fipto/refs/heads/main/openapi/fipto-assets-api-openapi.yml
- filename: fipto-automations-api-openapi.yml
  format: yaml
  label: Fipto Automations API
  slug: fipto-automations-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fipto/refs/heads/main/openapi/fipto-automations-api-openapi.yml
- filename: fipto-beneficiaries-api-openapi.yml
  format: yaml
  label: Fipto Beneficiaries API
  slug: fipto-beneficiaries-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fipto/refs/heads/main/openapi/fipto-beneficiaries-api-openapi.yml
- filename: fipto-companies-api-openapi.yml
  format: yaml
  label: Fipto Companies API
  slug: fipto-companies-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fipto/refs/heads/main/openapi/fipto-companies-api-openapi.yml
- filename: fipto-conversions-api-openapi.yml
  format: yaml
  label: Fipto Conversions API
  slug: fipto-conversions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fipto/refs/heads/main/openapi/fipto-conversions-api-openapi.yml
- filename: fipto-internal-transfers-api-openapi.yml
  format: yaml
  label: Fipto Internal Transfers API
  slug: fipto-internal-transfers-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fipto/refs/heads/main/openapi/fipto-internal-transfers-api-openapi.yml
- filename: fipto-payin-simulation-api-openapi.yml
  format: yaml
  label: Fipto Payin Simulation API
  slug: fipto-payin-simulation-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fipto/refs/heads/main/openapi/fipto-payin-simulation-api-openapi.yml
- filename: fipto-payment-links-api-openapi.yml
  format: yaml
  label: Fipto Payment links API
  slug: fipto-payment-links-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fipto/refs/heads/main/openapi/fipto-payment-links-api-openapi.yml
- filename: fipto-transactions-api-openapi.yml
  format: yaml
  label: Fipto Transactions API
  slug: fipto-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fipto/refs/heads/main/openapi/fipto-transactions-api-openapi.yml
- filename: fipto-travel-rule-api-openapi.yml
  format: yaml
  label: Fipto Travel Rule API
  slug: fipto-travel-rule-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fipto/refs/heads/main/openapi/fipto-travel-rule-api-openapi.yml
- filename: fipto-wallets-api-openapi.yml
  format: yaml
  label: Fipto Wallets API
  slug: fipto-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fipto/refs/heads/main/openapi/fipto-wallets-api-openapi.yml
consequence_counts:
  physical: 5
  read: 28
  write: 19
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 0
kind: agentic-access
layout: agentic-access
method: generated
name: Fipto Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /companies/{company_id}/aisp-pisp/wallets/{wallet_id}/payouts
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /companies/{company_id}/payment-links
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PATCH
  path: /companies/{company_id}/payment-links/{payment_link_id}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /companies/{company_id}/wallets/{wallet_id}/internal-transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /companies/{company_id}/wallets/{wallet_id}/payouts
operation_count: 52
overview: 'Fipto exposes 52 API operations that an AI agent could call, of which 24 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 28 read, 19 write, and 5 physical.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: Fipto
provider_slug: fipto
slug: fipto-agentic-access
source_filename: fipto-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-08-17'\nmethod: generated\nsource: openapi/fipto-customer-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\nsummary:\n  operations: 52\n  by_action_class:\n    connected: 28\n    acting: 24\n  by_consequence:\n    read: 28\n    write: 19\n    physical: 5\n  human_in_the_loop_required: 0\noperations:\n- path: /companies/{company_id}/assets\n  method: get\n  operationId: listAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{company_id}/request-usd\n  method: post\n  operationId: requestUsdOnboarding\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n \
  \   token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{company_id}/quotes\n  method: post\n  operationId: createAQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{company_id}/quotes/{quote_id}/status\n  method: patch\n  operationId: confirmQuoteStatus\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies\n  method: get\n  operationId: listCompaniesByUser\n  x-agentic-access:\n\
  \    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{company_id}\n  method: get\n  operationId: getCompany\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{company_id}/beneficiaries/file-conversion\n  method: post\n  operationId: validateBatchBeneficiary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{company_id}/beneficiaries/batch\n  method: post\n  operationId: createBatchBeneficiaries\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n\
  \    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{company_id}/beneficiaries\n  method: post\n  operationId: createBeneficiary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{company_id}/beneficiaries\n  method: get\n  operationId: listBeneficiaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{company_id}/beneficiaries/{beneficiary_id}\n  method: get\n  operationId: searchBeneficiaries\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit:\
  \ none\n- path: /companies/{company_id}/beneficiaries/{beneficiary_id}\n  method: delete\n  operationId: deleteBeneficiary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{company_id}/beneficiaries/{beneficiary_id}/verify\n  method: post\n  operationId: verifyBeneficiary\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{company_id}/beneficiaries/{beneficiary_id}/wallet-details/travel-rule\n  method: patch\n  operationId: updateBeneficiaryTravelRule\n  x-agentic-access:\n    action-class: acting\n \
  \   consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{company_id}/automations\n  method: get\n  operationId: listAutomations\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{company_id}/automations\n  method: post\n  operationId: createAutomation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{company_id}/automations/{automation_id}\n  method: get\n  operationId: getAutomation\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{company_id}/automations/{automation_id}\n  method: put\n  operationId: updateAutomation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{company_id}/automations/{automation_id}\n  method: delete\n  operationId: deleteAutomation\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{company_id}/wallets\n  method: post\n  operationId: createWalletByCompanyId\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{company_id}/wallets\n  method: get\n  operationId: listWallets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{company_id}/wallets/{wallet_id}\n  method: get\n  operationId: getWallet\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{company_id}/wallets/{wallet_id}\n  method: patch\n  operationId: updateWalletName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n\
  \      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{company_id}/transactions\n  method: get\n  operationId: searchTransactionsByCompanyId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{company_id}/operations\n  method: get\n  operationId: listOperationByOperationIds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{company_id}/transactions/{transaction_id}\n  method: get\n  operationId: getCompanyTransaction\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{company_id}/wallets/{wallet_id}/wallet-details\n  method: post\n  operationId: createWalletDetailsByWalletId\n  x-agentic-access:\n    action-class:\
  \ acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{company_id}/wallets/{wallet_id}/wallet-details\n  method: get\n  operationId: getWalletDetailsByWalletId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{company_id}/wallets/{wallet_id}/wallet-details/{wallet_details_id}\n  method: get\n  operationId: getWalletDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{company_id}/wallets/{wallet_id}/wallet-details/{wallet_details_id}\n  method: patch\n  operationId: updateWalletDetails\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n\
  \    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{company_id}/wallets/{wallet_id}/wallet-details/{wallet_details_id}/download\n  method: get\n  operationId: getWalletDetailsPDF\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{company_id}/payment-links/{payment_link_id}\n  method: get\n  operationId: getPaymentLink\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{company_id}/payment-links/{payment_link_id}\n  method: patch\n  operationId: updatePaymentLink\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{company_id}/payment-links\n  method: get\n  operationId: listPaymentLinks\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{company_id}/payment-links\n  method: post\n  operationId: createPaymentLinks\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{company_id}/wallets/{wallet_id}/payouts\n  method: post\n  operationId: initiatePayout\n  x-agentic-access:\n\
  \    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{company_id}/wallets/{wallet_id}/internal-transfers\n  method: post\n  operationId: createInternalTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{company_id}/pairs\n  method: get\n  operationId: getPairs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path:\
  \ /aisp-pisp\n  method: get\n  operationId: listAISPPISP\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{company_id}/aisp-pisp\n  method: post\n  operationId: createCompanyAISPPISP\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{company_id}/aisp-pisp\n  method: get\n  operationId: listCompanyAISPPISP\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{company_id}/aisp-pisp/{aisp_pisp_id}\n  method: get\n  operationId: getCompanyAISPPISP\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n\
  \    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{company_id}/aisp-pisp/{aisp_pisp_id}\n  method: delete\n  operationId: deleteCompanyAISPPISP\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{company_id}/aisp-pisp/wallets/{wallet_id}/payouts\n  method: post\n  operationId: initiatePayoutAISPPISP\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{company_id}/aisp-pisp/wallets\n  method: get\n  operationId:\
  \ listWalletAISPPISP\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{company_id}/aisp-pisp/wallets/{wallet_id}\n  method: get\n  operationId: getWalletAISPPISP\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{company_id}/aisp-pisp/transactions\n  method: get\n  operationId: searchTransactionsAISPPISPByCompanyId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{company_id}/aisp-pisp/transactions/{transaction_id}\n  method: get\n  operationId: getTransactionAISPPISP\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{company_id}/aisp-pisp/beneficiaries\n\
  \  method: get\n  operationId: listBeneficiariesAISPPISP\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{company_id}/aisp-pisp/beneficiaries/{beneficiary_id}\n  method: get\n  operationId: getBeneficiaryAISPPISP\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /companies/{company_id}/wallets/{wallet_id}/payin-simulation\n  method: post\n  operationId: simulatePayin\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /companies/{company_id}/conversions/{conversion_id}\n  method: get\n  operationId: getConversion\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fipto/refs/heads/main/agentic-access/fipto-agentic-access.yml
summary_line: 52 operations · 24 acting
tags:
- Company
- Blockchain
- Payments
- Stablecoins
- Banking
- Treasury
- Cross-Border Payments
- Digital Currency
- Fintech
- Wallets
---
