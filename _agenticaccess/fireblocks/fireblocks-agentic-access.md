---
acting_count: 160
action_class_counts:
  acting: 160
  connected: 143
api_specs:
- filename: fireblocks-vaults-api-openapi.yml
  format: yaml
  label: Fireblocks Vaults API
  slug: fireblocks-vaults-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-vaults-api-openapi.yml
- filename: fireblocks-transactions-api-openapi.yml
  format: yaml
  label: Fireblocks Transactions API
  slug: fireblocks-transactions-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-transactions-api-openapi.yml
- filename: fireblocks-wallets-api-openapi.yml
  format: yaml
  label: Fireblocks Whitelisted Wallets API
  slug: fireblocks-wallets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-wallets-api-openapi.yml
- filename: fireblocks-assets-api-openapi.yml
  format: yaml
  label: Fireblocks Blockchains and Assets API
  slug: fireblocks-assets-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-assets-api-openapi.yml
- filename: fireblocks-exchange-api-openapi.yml
  format: yaml
  label: Fireblocks Exchange and Fiat Accounts API
  slug: fireblocks-exchange-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-exchange-api-openapi.yml
- filename: fireblocks-tokenization-api-openapi.yml
  format: yaml
  label: Fireblocks Tokenization API
  slug: fireblocks-tokenization-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-tokenization-api-openapi.yml
- filename: fireblocks-contracts-api-openapi.yml
  format: yaml
  label: Fireblocks Smart Contracts API
  slug: fireblocks-contracts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-contracts-api-openapi.yml
- filename: fireblocks-staking-api-openapi.yml
  format: yaml
  label: Fireblocks Staking API
  slug: fireblocks-staking-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-staking-api-openapi.yml
- filename: fireblocks-nfts-api-openapi.yml
  format: yaml
  label: Fireblocks NFTs API
  slug: fireblocks-nfts-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-nfts-api-openapi.yml
- filename: fireblocks-payments-api-openapi.yml
  format: yaml
  label: Fireblocks Payments API
  slug: fireblocks-payments-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-payments-api-openapi.yml
- filename: fireblocks-network-api-openapi.yml
  format: yaml
  label: Fireblocks Network and Off-Exchange API
  slug: fireblocks-network-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-network-api-openapi.yml
- filename: fireblocks-compliance-api-openapi.yml
  format: yaml
  label: Fireblocks Compliance and Policy API
  slug: fireblocks-compliance-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-compliance-api-openapi.yml
- filename: fireblocks-gas-station-api-openapi.yml
  format: yaml
  label: Fireblocks Gas Station API
  slug: fireblocks-gas-station-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-gas-station-api-openapi.yml
- filename: fireblocks-workspace-api-openapi.yml
  format: yaml
  label: Fireblocks Workspace Management API
  slug: fireblocks-workspace-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-workspace-api-openapi.yml
- filename: fireblocks-webhooks-api-openapi.yml
  format: yaml
  label: Fireblocks Webhooks API
  slug: fireblocks-webhooks-api
  spec_type: OpenAPI
  url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/openapi/fireblocks-webhooks-api-openapi.yml
consequence_counts:
  physical: 42
  read: 143
  safety-critical: 3
  write: 115
description: Recommended x-agentic-access execution contracts, classified heuristically from the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind audience per deployment. See research/curity/agentic-governance/.
human_in_the_loop: 3
kind: agentic-access
layout: agentic-access
method: generated
name: Fireblocks Agentic Access
name_suffix: Agentic Access
notable_actions:
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PATCH
  path: /key_link/validation_keys/{keyId}
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: PUT
  path: /management/ota
- action_class: acting
  consequence: safety-critical
  human_in_the_loop: required
  method: POST
  path: /management/users/{id}/reset_device
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /exchange_accounts/{exchangeAccountId}/internal_transfer
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /fiat_accounts/{accountId}/deposit_from_linked_dda
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /nfts/ownership/tokens
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /nfts/ownership/tokens/spam
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /nfts/ownership/tokens/status
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /nfts/ownership/tokens/{id}/status
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /off_exchange/settlements/trader
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/payout
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/payout/{payoutId}/actions/execute
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/workflow_config
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: DELETE
  path: /payments/workflow_config/{configId}
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/workflow_execution
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /payments/workflow_execution/{workflowExecutionId}/actions/execute
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /policy/draft
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /smart-transfers
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /smart-transfers/settings/user-groups
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /smart-transfers/{ticketId}/cancel
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /smart-transfers/{ticketId}/expires-in
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /smart-transfers/{ticketId}/external-id
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /smart-transfers/{ticketId}/fulfill
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: PUT
  path: /smart-transfers/{ticketId}/submit
- action_class: acting
  consequence: physical
  human_in_the_loop: conditional
  method: POST
  path: /smart-transfers/{ticketId}/terms
operation_count: 303
overview: 'fireblocks exposes 303 API operations that an AI agent could call, of which 160 are state-changing ''acting'' operations. This is a recommended x-agentic-access execution contract — the scope, audience, consequence tier, short-lived token constraints, and escalation each action should carry before it is handed to an autonomous agent.


  By consequence: 143 read, 115 write, 42 physical, and 3 safety-critical.


  3 operations are classed safety-critical and should require human-in-the-loop approval at runtime.


  Contracts are classified heuristically from the provider''s OpenAPI and refresh on every APIs.io network build; audience is bound per deployment. The model follows Curity''s Access Intelligence (apidays Munich 2026). Browse every provider''s agent contracts at [agentic-access.apis.io](https://apis.io/agentic-access/).'
provider_name: fireblocks
provider_slug: fireblocks
slug: fireblocks-agentic-access
source_filename: fireblocks-agentic-access.yml
source_heading: Agentic Access
source_url: ''
source_yaml: "generated: '2026-07-15'\nmethod: generated\nsource: openapi/fireblocks-assets-api-openapi.yml, openapi/fireblocks-compliance-api-openapi.yml,\n  openapi/fireblocks-contracts-api-openapi.yml, openapi/fireblocks-exchange-api-openapi.yml,\n  openapi/fireblocks-gas-station-api-openapi.yml, openapi/fireblocks-network-api-openapi.yml,\n  openapi/fireblocks-nfts-api-openapi.yml, openapi/fireblocks-payments-api-openapi.yml, openapi/fireblocks-staking-api-openapi.yml,\n  openapi/fireblocks-tokenization-api-openapi.yml, openapi/fireblocks-transactions-api-openapi.yml,\n  openapi/fireblocks-vaults-api-openapi.yml, openapi/fireblocks-wallets-api-openapi.yml, openapi/fireblocks-webhooks-api-openapi.yml,\n  openapi/fireblocks-workspace-api-openapi.yml\ndescription: Recommended x-agentic-access execution contracts, classified heuristically from\n  the OpenAPI. A governance starting point for exposing this API to AI agents — review and bind\n  audience per deployment. See research/curity/agentic-governance/.\n\
  summary:\n  operations: 303\n  by_action_class:\n    connected: 143\n    acting: 160\n  by_consequence:\n    read: 143\n    write: 115\n    physical: 42\n    safety-critical: 3\n  human_in_the_loop_required: 3\noperations:\n- path: /assets\n  method: get\n  operationId: listAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets\n  method: post\n  operationId: registerNewAsset\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/{id}\n  method: get\n  operationId: getAsset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /assets/{id}\n\
  \  method: patch\n  operationId: updateAssetUserMetadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /assets/prices/{id}\n  method: post\n  operationId: setAssetPrice\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /blockchains\n  method: get\n  operationId: listBlockchains\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /blockchains/{id}\n  method: get\n  operationId: getBlockchain\n  x-agentic-access:\n    action-class:\
  \ connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /transactions/validate_address/{assetId}/{address}\n  method: get\n  operationId: validateAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /estimate_network_fee\n  method: get\n  operationId: estimateNetworkFee\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /supported_assets\n  method: get\n  operationId: getSupportedAssets\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /screening/travel_rule/transaction/validate\n  method: post\n  operationId: validateTravelRuleTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /screening/travel_rule/transaction/validate/full\n  method: post\n  operationId: validateFullTravelRuleTransaction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /screening/travel_rule/vasp/{did}\n  method: get\n  operationId: getVASPByDID\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /screening/travel_rule/vasp\n  method: get\n  operationId: getVASPs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject:\
  \ optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /screening/travel_rule/vasp/update\n  method: put\n  operationId: updateVasp\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /screening/travel_rule/post_screening_policy\n  method: get\n  operationId: getPostScreeningPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /screening/travel_rule/screening_policy\n  method: get\n  operationId: getScreeningPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /screening/travel_rule/vault/{vaultAccountId}/vasp\n  method: get\n\
  \  operationId: getVaspForVault\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /screening/travel_rule/vault/{vaultAccountId}/vasp\n  method: post\n  operationId: setVaspForVault\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /screening/travel_rule/policy_configuration\n  method: get\n  operationId: getScreeningConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /screening/travel_rule/policy_configuration\n  method: put\n  operationId: updateTravelRuleConfig\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n \
  \   subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /screening/aml/policy_configuration\n  method: get\n  operationId: getAmlScreeningConfiguration\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /screening/aml/policy_configuration\n  method: put\n  operationId: updateAmlScreeningConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /screening/aml/screening_policy\n  method: get\n  operationId: getAmlScreeningPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence:\
  \ read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /screening/aml/post_screening_policy\n  method: get\n  operationId: getAmlPostScreeningPolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /screening/configurations\n  method: put\n  operationId: updateScreeningConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /screening/transaction/{txId}/bypass_screening_policy\n  method: post\n  operationId: retryRejectedTransactionBypassScreeningChecks\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n\
  \      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /screening/transaction/{txId}\n  method: get\n  operationId: getScreeningFullDetails\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /screening/aml/verdict/manual\n  method: post\n  operationId: setAmlVerdict\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tap/active_policy\n  method: get\n  operationId: getActivePolicy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tap/draft\n  method: get\n  operationId: getDraft\n \
  \ x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tap/draft\n  method: put\n  operationId: updateDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tap/draft\n  method: post\n  operationId: publishDraft\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tap/publish\n  method: post\n  operationId: publishPolicyRules\n  x-agentic-access:\n    action-class: acting\n\
  \    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /policy/active_policy\n  method: get\n  operationId: getActiveV2Policy\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /policy/draft\n  method: get\n  operationId: getV2Draft\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /policy/draft\n  method: put\n  operationId: updateV2Draft\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /policy/draft\n  method: post\n  operationId: publishV2Draft\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tokenization/templates\n  method: get\n  operationId: getContractTemplates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tokenization/templates\n  method: post\n  operationId: uploadContractTemplate\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n\
  \      - abnormal\n      - high-value\n    audit: required\n- path: /tokenization/templates/{contractTemplateId}\n  method: get\n  operationId: getContractTemplateById\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tokenization/templates/{contractTemplateId}\n  method: delete\n  operationId: deleteContractTemplateById\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tokenization/templates/{contractTemplateId}/constructor\n  method: get\n  operationId: getConstructorByContractTemplateId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tokenization/templates/{contractTemplateId}/function\n\
  \  method: get\n  operationId: getFunctionAbiByContractTemplateId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tokenization/templates/{contractTemplateId}/deploy\n  method: post\n  operationId: deployContract\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tokenization/contracts\n  method: get\n  operationId: getDeployedContracts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tokenization/contracts/{id}\n  method: get\n  operationId: getDeployedContractById\n  x-agentic-access:\n \
  \   action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tokenization/contracts/{assetId}/{contractAddress}\n  method: get\n  operationId: getDeployedContractByAddress\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /tokenization/contracts/fetch_abi\n  method: post\n  operationId: fetchContractAbi\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /tokenization/contracts/abi\n  method: post\n  operationId: addContractABI\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n  \
  \  audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contract_interactions/base_asset_id/{baseAssetId}/contract_address/{contractAddress}/functions\n  method: get\n  operationId: getDeployedContractAbi\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /contract_interactions/base_asset_id/{baseAssetId}/contract_address/{contractAddress}/functions/read\n  method: post\n  operationId: readCallFunction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contract_interactions/base_asset_id/{baseAssetId}/contract_address/{contractAddress}/functions/write\n\
  \  method: post\n  operationId: writeCallFunction\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /contract_interactions/base_asset_id/{baseAssetId}/tx_hash/{txHash}/receipt\n  method: get\n  operationId: getTransactionReceipt\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connections\n  method: get\n  operationId: get\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connections/wc\n  method: post\n  operationId: create\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n\
  \      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connections/wc/{id}\n  method: put\n  operationId: submit\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connections/wc/{id}\n  method: delete\n  operationId: remove\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /exchange_accounts\n  method: get\n  operationId: getExchangeAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n  \
  \  subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exchange_accounts\n  method: post\n  operationId: addExchangeAccount\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /exchange_accounts/paged\n  method: get\n  operationId: getPagedExchangeAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exchange_accounts/{exchangeAccountId}\n  method: get\n  operationId: getExchangeAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exchange_accounts/{exchangeAccountId}/internal_transfer\n  method: post\n  operationId:\
  \ internalTransfer\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /exchange_accounts/{exchangeAccountId}/convert\n  method: post\n  operationId: convertAssets\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /exchange_accounts/{exchangeAccountId}/{assetId}\n  method: get\n  operationId: getExchangeAccountAsset\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /exchange_accounts/credentials_public_key\n\
  \  method: get\n  operationId: getExchangeAccountsCredentialsPublicKey\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fiat_accounts\n  method: get\n  operationId: getFiatAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fiat_accounts/{accountId}\n  method: get\n  operationId: getFiatAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /fiat_accounts/{accountId}/redeem_to_linked_dda\n  method: post\n  operationId: redeemFundsToLinkedDDA\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      -\
  \ abnormal\n      - high-value\n    audit: required\n- path: /fiat_accounts/{accountId}/deposit_from_linked_dda\n  method: post\n  operationId: depositFundsFromLinkedDDA\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /connected_accounts\n  method: get\n  operationId: getConnectedAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connected_accounts/{accountId}\n  method: get\n  operationId: getConnectedAccount\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connected_accounts/{accountId}/balances\n\
  \  method: get\n  operationId: getConnectedAccountBalances\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connected_accounts/{accountId}/rates\n  method: get\n  operationId: getConnectedAccountRates\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /connected_accounts/{accountId}/manifest/capabilities/trading/pairs\n  method: get\n  operationId: getConnectedAccountTradingPairs\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trading/providers\n  method: get\n  operationId: getTradingProviders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trading/quotes\n  method:\
  \ post\n  operationId: createQuote\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /trading/orders\n  method: post\n  operationId: createOrder\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /trading/orders\n  method: get\n  operationId: getOrders\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /trading/orders/{orderId}\n  method: get\n  operationId: getOrder\n\
  \  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gas_station\n  method: get\n  operationId: getGasStationInfo\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gas_station/{assetId}\n  method: get\n  operationId: getGasStationByAssetId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /gas_station/configuration\n  method: put\n  operationId: updateGasStationConfiguration\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /gas_station/configuration/{assetId}\n\
  \  method: put\n  operationId: updateGasStationConfigurationByAssetId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /network_connections\n  method: get\n  operationId: getNetworkConnections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /network_connections\n  method: post\n  operationId: createNetworkConnection\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /network_connections/{connectionId}/set_routing_policy\n\
  \  method: patch\n  operationId: setRoutingPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /network_connections/{connectionId}/is_third_party_routing/{assetType}\n  method: get\n  operationId: checkThirdPartyRouting\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /network_connections/{connectionId}\n  method: get\n  operationId: getNetwork\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /network_connections/{connectionId}\n  method: delete\n  operationId: deleteNetworkConnection\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /network_ids\n  method: get\n  operationId: getNetworkIds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /network_ids\n  method: post\n  operationId: createNetworkId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /network_ids/routing_policy_asset_groups\n  method: get\n  operationId: getRoutingPolicyAssetGroups\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl:\
  \ 3600\n    audit: none\n- path: /network_ids/search\n  method: get\n  operationId: searchNetworkIds\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /network_ids/{networkId}\n  method: get\n  operationId: getNetworkId\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /network_ids/{networkId}\n  method: delete\n  operationId: deleteNetworkId\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /network_ids/{networkId}/set_routing_policy\n  method: patch\n  operationId: setNetworkIdRoutingPolicy\n  x-agentic-access:\n    action-class: acting\n    consequence:\
  \ write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /network_ids/{networkId}/set_discoverability\n  method: patch\n  operationId: setNetworkIdDiscoverability\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /network_ids/{networkId}/set_name\n  method: patch\n  operationId: setNetworkIdName\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /off_exchange/add\n\
  \  method: post\n  operationId: addOffExchange\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /off_exchange/remove\n  method: post\n  operationId: removeOffExchange\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    audience: null\n    token:\n      max-ttl: 900\n    escalation:\n      human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /off_exchange/settlements/trader\n  method: post\n  operationId: settleOffExchangeTrades\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n \
  \     human-in-the-loop: conditional\n      triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /off_exchange/settlements/transactions\n  method: get\n  operationId: getOffExchangeSettlementTransactions\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /off_exchange/collateral_accounts/{mainExchangeAccountId}\n  method: get\n  operationId: getOffExchangeCollateralAccounts\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nfts/ownership/tokens\n  method: put\n  operationId: updateOwnershipTokens\n  x-agentic-access:\n    action-class: acting\n    consequence: physical\n    subject: required\n    audience: null\n    token:\n      max-ttl: 300\n      exchange: true\n      purpose-required: true\n    escalation:\n      human-in-the-loop: conditional\n     \
  \ triggers:\n      - abnormal\n      - high-value\n    audit: required\n- path: /nfts/ownership/tokens\n  method: get\n  operationId: getOwnershipTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nfts/ownership/assets\n  method: get\n  operationId: listOwnedTokens\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nfts/ownership/collections\n  method: get\n  operationId: listOwnedCollections\n  x-agentic-access:\n    action-class: connected\n    consequence: read\n    subject: optional\n    token:\n      max-ttl: 3600\n    audit: none\n- path: /nfts/tokens/{id}\n  method: put\n  operationId: refreshNFTMetadata\n  x-agentic-access:\n    action-class: acting\n    consequence: write\n    subject: required\n    a\n\n# --- truncated at 32 KB (90 KB total) ---\n# Full source: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/agentic-access/fireblocks-agentic-access.yml\n"
source_yaml_url: https://raw.githubusercontent.com/api-evangelist/fireblocks/refs/heads/main/agentic-access/fireblocks-agentic-access.yml
summary_line: 303 operations · 160 acting · 3 human-in-the-loop
tags: []
---
